# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

An Android SMS messaging app (Kotlin). It is a fork of [Fossify Messages](https://github.com/FossifyOrg/Messages) — the entire base app lives under the `org.fossify.messages` package (`app/src/main`). Traccar's value-add is an **HTTP + Firebase SMS gateway** that lets a server send SMS through the phone. That gateway code lives only in the `traccar` build flavor under `org.traccar.gateway` (`app/src/traccar`).

When working on app/messaging features, you are editing upstream Fossify code. When working on the gateway, you are editing the small Traccar-specific layer.

## Build & checks

Java 17, Gradle (wrapper), AGP 9.x, compileSdk 36, minSdk 26. The `traccar` flavor is the default and the only one that matters for releases.

```bash
./gradlew assembleTraccarDebug          # debug build (what CI build.yml runs)
./gradlew :app:assembleTraccarRelease   # release build (needs signing, see below)
./gradlew detekt                        # static analysis — maxIssues=0, fails on any new issue
./gradlew :app:lintTraccarRelease       # Android lint — abortOnError=true
./gradlew clean
```

- **Build a specific flavor** by swapping the flavor name: `assemble{Core,Foss,Gplay,Traccar}{Debug,Release}`.
- **detekt** uses `detekt.yml` + `app/detekt-baseline.xml`. Pre-existing issues are baselined; new code must be clean. Regenerate baseline only deliberately with `./gradlew detektBaseline`.
- **lint** uses `lint.xml` + `app/lint-baseline.xml` (same baseline pattern).
- **No unit or instrumented tests exist** in the repo. CI verification is a smoke test: the release workflow installs the APK on an emulator, launches it, and asserts the process didn't crash. There is no `./gradlew test` to run.

## Product flavors

Defined in `app/build.gradle.kts` under `productFlavors` (dimension `variants`): `core`, `foss`, `gplay`, `traccar` (default).

- **Only `traccar`** pulls in Jetty (`jetty-server`, `javax-servlet`) and Firebase (`traccarImplementation` deps) — see the `"traccarImplementation"(...)` lines. The other flavors are inherited from upstream and largely inert here.
- `traccar` **overrides** the base version (`gradle.properties` has `VERSION_NAME=1.8.0`/`VERSION_CODE=20`, `APP_ID=org.fossify.messages`) with `applicationId = org.traccar.gateway`, `versionName = 7.0.1`, `versionCode = 22`. **Bump the version in the `traccar` flavor block, not `gradle.properties`.**
- `app/src/traccar/` carries its own `AndroidManifest.xml` (registers the gateway components + foreground-service permissions) and `google-services.json` for Firebase.

## Gateway architecture (`org.traccar.gateway`)

The gateway exposes two independent paths to trigger an SMS send, both ending in the same `SmsManager` call:

1. **Local HTTP** — `GatewayService` (a foreground `Service`, port `8082`) starts `GatewayServer`, a Jetty `Server`. `POST /` with header `Authorization: <key>` and JSON body `{"to": ..., "message": ..., "slot": <optional sim slot>}`. The key is `gateway_api_key` in default `SharedPreferences`, auto-generated as a UUID by `GatewayActivity` on first view. `handleGet()` returns API docs HTML.
2. **Cloud / Firebase** — `GatewayMessagingService` (a `FirebaseMessagingService`) receives FCM data messages (`phone`, `message`, `slot`) and sends without any local server running.

Both call `GatewayServiceUtil.sendMessage(context, phone, message, slot)`, which picks the SIM via `SubscriptionManager` when `slot` is given (else `SmsManager.getDefault()`) and uses `divideMessage` + `sendMultipartTextMessage`. `GatewayActivity` is the settings UI: shows the local key, the FCM token, the device's LAN endpoint URLs, and a toggle to start/stop `GatewayService`.

## App architecture (upstream Fossify, `org.fossify.messages`)

Standard Android view-based app (View Binding, no Compose). Key areas under `app/src/main/kotlin/org/fossify/messages/`:

- `messaging/` — send/receive core. `MessagingUtils` (insert into telephony DB, MMS), `SmsSender`/`Messaging.kt` (`sendMessageCompat`), `SmsManager.kt`, status-report intents.
- `databases/` — Room (`MessagesDatabase`, KSP-generated; schema at `app/schemas`). DAOs: Messages, Conversations, Attachments, Drafts. Holds local cache/metadata on top of the system telephony provider.
- `activities/`, `adapters/`, `dialogs/`, `receivers/`, `models/`, `helpers/`, `extensions/` — UI and supporting code. Depends heavily on `org.fossify:commons`.

## Signing

Release signing reads `keystore.properties` (see `keystore.properties_sample`) if present, otherwise the `SIGNING_KEY_ALIAS` / `SIGNING_KEY_PASSWORD` / `SIGNING_STORE_FILE` / `SIGNING_STORE_PASSWORD` env vars (used by CI). Missing both → unsigned build with a warning. Release CI (`.github/workflows/release.yml`, on `v*` tags) builds, smoke-tests on an emulator, uploads to Google Play production, and creates a GitHub release.

## graphify

This project has a knowledge graph at graphify-out/ with god nodes, community structure, and cross-file relationships.

Rules:
- For codebase questions, first run `graphify query "<question>"` when graphify-out/graph.json exists. Use `graphify path "<A>" "<B>"` for relationships and `graphify explain "<concept>"` for focused concepts. These return a scoped subgraph, usually much smaller than GRAPH_REPORT.md or raw grep output.
- If graphify-out/wiki/index.md exists, use it for broad navigation instead of raw source browsing.
- Read graphify-out/GRAPH_REPORT.md only for broad architecture review or when query/path/explain do not surface enough context.
- After modifying code, run `graphify update .` to keep the graph current (AST-only, no API cost).
