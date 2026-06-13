# Graph Report - .  (2026-06-13)

## Corpus Check
- Corpus is ~39,654 words - fits in a single context window. You may not need a graph.

## Summary
- 1481 nodes · 2704 edges · 90 communities (73 shown, 17 thin omitted)
- Extraction: 93% EXTRACTED · 7% INFERRED · 0% AMBIGUOUS · INFERRED: 187 edges (avg confidence: 0.8)
- Token cost: 554,785 input · 0 output

## Community Hubs (Navigation)
- [[_COMMUNITY_Thread & Autocomplete Adapters|Thread & Autocomplete Adapters]]
- [[_COMMUNITY_Blocked Keywords Management|Blocked Keywords Management]]
- [[_COMMUNITY_Main Conversations Screen|Main Conversations Screen]]
- [[_COMMUNITY_Contacts Selection Adapter|Contacts Selection Adapter]]
- [[_COMMUNITY_Conversation Query Extensions|Conversation Query Extensions]]
- [[_COMMUNITY_Attachment & Settings Types|Attachment & Settings Types]]
- [[_COMMUNITY_Attachments Adapter|Attachments Adapter]]
- [[_COMMUNITY_MMSSMS Backup Types|MMS/SMS Backup Types]]
- [[_COMMUNITY_New Conversation Screen|New Conversation Screen]]
- [[_COMMUNITY_Messages DAO (Room)|Messages DAO (Room)]]
- [[_COMMUNITY_Settings Screen|Settings Screen]]
- [[_COMMUNITY_Thread (Conversation) Screen|Thread (Conversation) Screen]]
- [[_COMMUNITY_Recycle Bin & Deletion Extensions|Recycle Bin & Deletion Extensions]]
- [[_COMMUNITY_VCard Viewer Screen|VCard Viewer Screen]]
- [[_COMMUNITY_Message Import Flow|Message Import Flow]]
- [[_COMMUNITY_Backup Serialization (Polymorphic)|Backup Serialization (Polymorphic)]]
- [[_COMMUNITY_Message Notification Context|Message Notification Context]]
- [[_COMMUNITY_Broadcast Receivers (SMS Actions)|Broadcast Receivers (SMS Actions)]]
- [[_COMMUNITY_ArchivedRecycleBin Conversation Adapters|Archived/RecycleBin Conversation Adapters]]
- [[_COMMUNITY_Conversations Adapter|Conversations Adapter]]
- [[_COMMUNITY_JSON Object Extensions|JSON Object Extensions]]
- [[_COMMUNITY_MMS Sent Receiver|MMS Sent Receiver]]
- [[_COMMUNITY_Archived Conversations Screen|Archived Conversations Screen]]
- [[_COMMUNITY_Recycle Bin Conversations Screen|Recycle Bin Conversations Screen]]
- [[_COMMUNITY_ConversationMMS Query Extensions|Conversation/MMS Query Extensions]]
- [[_COMMUNITY_Conversations DAO|Conversations DAO]]
- [[_COMMUNITY_Thread Participants Setup|Thread Participants Setup]]
- [[_COMMUNITY_Base Conversations Adapter|Base Conversations Adapter]]
- [[_COMMUNITY_Room Database Definition|Room Database Definition]]
- [[_COMMUNITY_MMSSMS Backup Writer|MMS/SMS Backup Writer]]
- [[_COMMUNITY_Conversation Details Screen|Conversation Details Screen]]
- [[_COMMUNITY_Build Config & Project Metadata|Build Config & Project Metadata]]
- [[_COMMUNITY_Image Compression|Image Compression]]
- [[_COMMUNITY_Shortcut Helper|Shortcut Helper]]
- [[_COMMUNITY_Message Sending (Thread)|Message Sending (Thread)]]
- [[_COMMUNITY_Cursor→JSON  Gson Deserializer|Cursor→JSON / Gson Deserializer]]
- [[_COMMUNITY_Message Models|Message Models]]
- [[_COMMUNITY_Attachment Composing (Thread)|Attachment Composing (Thread)]]
- [[_COMMUNITY_Scheduled Message UI|Scheduled Message UI]]
- [[_COMMUNITY_Attachment Picker Intents|Attachment Picker Intents]]
- [[_COMMUNITY_MMS Sender & Notification Extensions|MMS Sender & Notification Extensions]]
- [[_COMMUNITY_Gateway Foreground Service|Gateway Foreground Service]]
- [[_COMMUNITY_MIME Type String Helpers|MIME Type String Helpers]]
- [[_COMMUNITY_Room Type Converters|Room Type Converters]]
- [[_COMMUNITY_SMS Intent Parser|SMS Intent Parser]]
- [[_COMMUNITY_Gateway HTTP Server (Jetty)|Gateway HTTP Server (Jetty)]]
- [[_COMMUNITY_Thread Items Sealed Types|Thread Items Sealed Types]]
- [[_COMMUNITY_Conversation View Binding|Conversation View Binding]]
- [[_COMMUNITY_Message Details Dialog|Message Details Dialog]]
- [[_COMMUNITY_SimpleContact Extensions|SimpleContact Extensions]]
- [[_COMMUNITY_Attachment SMIL Parser|Attachment SMIL Parser]]
- [[_COMMUNITY_Drafts DAO|Drafts DAO]]
- [[_COMMUNITY_Conversation Models|Conversation Models]]
- [[_COMMUNITY_Gateway Config Activity|Gateway Config Activity]]
- [[_COMMUNITY_VCard Model|VCard Model]]
- [[_COMMUNITY_SMS Status Sent Receiver|SMS Status Sent Receiver]]
- [[_COMMUNITY_Gateway SMS Send Flow|Gateway SMS Send Flow]]
- [[_COMMUNITY_Activity Launch Extensions|Activity Launch Extensions]]
- [[_COMMUNITY_Collections Extensions|Collections Extensions]]
- [[_COMMUNITY_Conversation Persistence Extensions|Conversation Persistence Extensions]]
- [[_COMMUNITY_Attachment Selection Model|Attachment Selection Model]]
- [[_COMMUNITY_Thread Message Loading|Thread Message Loading]]
- [[_COMMUNITY_Scheduled Message Alarms|Scheduled Message Alarms]]
- [[_COMMUNITY_SimpleActivity Base|SimpleActivity Base]]
- [[_COMMUNITY_Message Label Helpers|Message Label Helpers]]
- [[_COMMUNITY_App Class & Messaging Cache|App Class & Messaging Cache]]
- [[_COMMUNITY_Adapter RecyclerView State|Adapter RecyclerView State]]
- [[_COMMUNITY_Drafts Extensions|Drafts Extensions]]
- [[_COMMUNITY_URI File Extensions|URI File Extensions]]
- [[_COMMUNITY_Attachments DAO|Attachments DAO]]
- [[_COMMUNITY_Message Attachments DAO|Message Attachments DAO]]
- [[_COMMUNITY_Gateway FCM Service|Gateway FCM Service]]
- [[_COMMUNITY_Attachment Models|Attachment Models]]
- [[_COMMUNITY_Rename Conversation Dialog|Rename Conversation Dialog]]
- [[_COMMUNITY_Conversation Update Extensions|Conversation Update Extensions]]
- [[_COMMUNITY_Event Bus Events|Event Bus Events]]
- [[_COMMUNITY_Module 76|Module 76]]
- [[_COMMUNITY_Module 77|Module 77]]
- [[_COMMUNITY_Module 78|Module 78]]
- [[_COMMUNITY_Module 79|Module 79]]
- [[_COMMUNITY_Module 82|Module 82]]
- [[_COMMUNITY_Module 83|Module 83]]
- [[_COMMUNITY_Module 84|Module 84]]
- [[_COMMUNITY_Module 85|Module 85]]
- [[_COMMUNITY_Module 86|Module 86]]
- [[_COMMUNITY_Module 88|Module 88]]
- [[_COMMUNITY_Module 89|Module 89]]

## God Nodes (most connected - your core abstractions)
1. `ThreadActivity` - 112 edges
2. `MainActivity` - 45 edges
3. `ThreadAdapter` - 41 edges
4. `SettingsActivity` - 34 edges
5. `Long` - 33 edges
6. `BaseConversationsAdapter` - 30 edges
7. `MessagesDao` - 28 edges
8. `ConversationsAdapter` - 22 edges
9. `ManageBlockedKeywordsAdapter` - 22 edges
10. `ArchivedConversationsActivity` - 21 edges

## Surprising Connections (you probably didn't know these)
- `Release Workflow` --references--> `traccar Product Flavor`  [INFERRED]
  .github/workflows/release.yml → app/build.gradle.kts
- `Traccar SMS Gateway` --conceptually_related_to--> `traccar Product Flavor`  [INFERRED]
  README.md → app/build.gradle.kts
- `ArchivedConversationsActivity` --semantically_similar_to--> `RecycleBinConversationsActivity`  [INFERRED] [semantically similar]
  app/src/main/kotlin/org/fossify/messages/activities/ArchivedConversationsActivity.kt → app/src/main/kotlin/org/fossify/messages/activities/RecycleBinConversationsActivity.kt
- `ArchivedConversationsAdapter` --semantically_similar_to--> `ConversationsAdapter`  [INFERRED] [semantically similar]
  app/src/main/kotlin/org/fossify/messages/adapters/ArchivedConversationsAdapter.kt → app/src/main/kotlin/org/fossify/messages/adapters/ConversationsAdapter.kt
- `ThreadAdapter` --semantically_similar_to--> `AttachmentsAdapter`  [INFERRED] [semantically similar]
  app/src/main/kotlin/org/fossify/messages/adapters/ThreadAdapter.kt → app/src/main/kotlin/org/fossify/messages/adapters/AttachmentsAdapter.kt

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Traccar release build, smoke-test and publish pipeline** — workflows_release, app_build_gradle_traccar_flavor, app_build_gradle_release_signing [EXTRACTED 0.85]
- **EventBus RefreshConversations subscribers** — activities_mainactivity_mainactivity, activities_archivedconversationsactivity_archivedconversationsactivity, activities_recyclebinconversationsactivity_recyclebinconversationsactivity, models_events_refreshconversations, concept_eventbus_refresh_conversations [INFERRED 0.85]
- **Conversation list activities launching ThreadActivity** — activities_mainactivity_mainactivity, activities_archivedconversationsactivity_archivedconversationsactivity, activities_recyclebinconversationsactivity_recyclebinconversationsactivity, activities_threadactivity_threadactivity [INFERRED 0.75]
- **Conversations adapter family sharing BaseConversationsAdapter** — adapters_baseconversationsadapter_baseconversationsadapter, adapters_archivedconversationsadapter_archivedconversationsadapter, adapters_conversationsadapter_conversationsadapter, adapters_recyclebinconversationsadapter_recyclebinconversationsadapter [EXTRACTED 1.00]
- **Blocked keyword management dialogs and adapter** — dialogs_addblockedkeyworddialog_addblockedkeyworddialog, dialogs_exportblockedkeywordsdialog_exportblockedkeywordsdialog, dialogs_manageblockedkeywordsadapter_manageblockedkeywordsadapter [INFERRED 0.85]
- **Message export/import backup flow** — dialogs_exportmessagesdialog_exportmessagesdialog, dialogs_importmessagesdialog_importmessagesdialog, helpers_messagesreader_messagesreader, helpers_messagesimporter_messagesimporter [INFERRED 0.85]
- **Conversation listing query pipeline** — extensions_context_getconversations, extensions_context_getthreadphonenumbers, extensions_context_getthreadcontactnames, extensions_context_getunreadcountsbythread [INFERRED 0.85]
- **MMS message assembly** — extensions_context_getmms, extensions_context_getmmsattachment, extensions_context_getmmssender, extensions_context_getthreadparticipants [INFERRED 0.85]
- **Message import pipeline: importer reads, writer persists, conversations refresh** — helpers_messagesimporter_restoremessages, helpers_messageswriter, helpers_constants_refreshconversations [INFERRED 0.85]
- **Blocked keywords export/import/filter via Config** — helpers_blockedkeywordsexporter, helpers_blockedkeywordsimporter, helpers_receiverutils_ismessagefilteredout, helpers_config [INFERRED 0.75]
- **Notification display creates/reports conversation shortcuts** — helpers_notificationhelper_showmessagenotification, helpers_shortcuthelper, helpers_config [INFERRED 0.85]
- **Remote SMS dispatch flow: FCM/HTTP request to gateway then native SmsManager send** — gateway_gatewaymessagingservice_gatewaymessagingservice, gateway_gatewayserver_gatewayserver, gateway_gatewayservice_gatewayservice, gateway_gatewayserviceutil_gatewayserviceutil [EXTRACTED 0.95]
- **In-app SMS send pipeline: compat dispatcher to MessagingUtils persistence to SmsSender to SmsManager** — messaging_messaging_sendmessagecompat, messaging_messagingutils_sendsmsmessage, messaging_smssender_sendmessage, messaging_smsmanager_getsmsmanager [EXTRACTED 0.95]
- **Backup serialization model family** — models_messagesbackup_messagesbackup, models_smsbackup_smsbackup, models_mmsbackup_mmsbackup, models_backuptype_backuptype, models_exportedmessage_exportedmessage [INFERRED 0.85]
- **Thread item hierarchy** — models_threaditems_threaditem, models_message_message [EXTRACTED 1.00]
- **SMS/MMS send status callback receivers** — receivers_sendstatusreceiver_sendstatusreceiver, receivers_mmssentreceiver_mmssentreceiver, receivers_smsstatussentreceiver_smsstatussentreceiver, receivers_smsstatusdeliveredreceiver_smsstatusdeliveredreceiver [INFERRED 0.85]
- **Inbound SMS/MMS receive and notify flow** — receivers_smsreceiver_smsreceiver, receivers_mmsreceiver_mmsreceiver, helpers_receiverutils_receiverutils [INFERRED 0.85]
- **Notification action receivers (reply/read/delete)** — receivers_directreplyreceiver_directreplyreceiver, receivers_markasreadreceiver_markasreadreceiver, receivers_deletesmsreceiver_deletesmsreceiver [INFERRED 0.75]

## Communities (90 total, 17 thin omitted)

### Community 0 - "Thread & Autocomplete Adapters"
Cohesion: 0.05
Nodes (28): AutoCompleteTextViewAdapter, ThreadAdapter, ThreadItemDiffCallback, ThreadViewHolder, Int, SimpleContact, View, ViewGroup (+20 more)

### Community 1 - "Blocked Keywords Management"
Cohesion: 0.05
Nodes (22): ManageBlockedKeywordsActivity, Bundle, OutputStream, String, Uri, Int, Menu, String (+14 more)

### Community 2 - "Main Conversations Screen"
Cohesion: 0.07
Nodes (18): MainActivity, SplashActivity, Any, ArrayList, Boolean, Bundle, Conversation, EventBus (+10 more)

### Community 3 - "Contacts Selection Adapter"
Cohesion: 0.05
Nodes (18): ContactsAdapter, SearchResultsAdapter, ArrayList, Int, Menu, SimpleContact, View, ViewGroup (+10 more)

### Community 4 - "Conversation Query Extensions"
Cohesion: 0.06
Nodes (31): Boolean, Context, Conversation, Int, List, Long, Set, String (+23 more)

### Community 5 - "Attachment & Settings Types"
Cohesion: 0.08
Nodes (30): Attachment, Boolean, Int, Intent, List, Long, Set, Settings (+22 more)

### Community 6 - "Attachments Adapter"
Cohesion: 0.10
Nodes (19): AttachmentDiffCallback, AttachmentsAdapter, AttachmentsViewHolder, VCardContactViewHolder, VCardPropertyViewHolder, VCardViewerAdapter, Boolean, Int (+11 more)

### Community 7 - "MMS/SMS Backup Types"
Cohesion: 0.11
Nodes (17): AlertDialog, Uri, AlertDialog, Boolean, DateTime, Int, Boolean, List (+9 more)

### Community 8 - "New Conversation Screen"
Cohesion: 0.09
Nodes (22): NewConversationActivity, ArrayList, Boolean, Bundle, SimpleContact, String, Attachment, Boolean (+14 more)

### Community 9 - "Messages DAO (Room)"
Cohesion: 0.13
Nodes (7): Int, List, Long, Message, String, MessagesDao, RecycleBinMessage

### Community 10 - "Settings Screen"
Cohesion: 0.11
Nodes (4): SettingsActivity, Bundle, app Config preferences, ExportMessagesDialog

### Community 11 - "Thread (Conversation) Screen"
Cohesion: 0.11
Nodes (7): ThreadActivity, Boolean, Bundle, Conversation, EventBus, Float, MenuItem

### Community 12 - "Recycle Bin & Deletion Extensions"
Cohesion: 0.13
Nodes (28): Boolean, List, Long, MessageAttachment, Unit, checkAndDeleteOldRecycleBinMessages(), clearExpiredScheduledMessages(), deleteConversation() (+20 more)

### Community 13 - "VCard Viewer Screen"
Cohesion: 0.08
Nodes (24): VCardViewerActivity, Activity, Bundle, List, Uri, VCard, VCardPropertyWrapper, VCardWrapper (+16 more)

### Community 14 - "Message Import Flow"
Cohesion: 0.09
Nodes (17): Boolean, List, MessagesBackup, SmsBackup, String, Uri, ImportMessagesDialog, refreshConversations() (+9 more)

### Community 15 - "Backup Serialization (Polymorphic)"
Cohesion: 0.08
Nodes (18): JsonElement, ContentValues, ContentValues, Boolean, ContentValues, ContentValues, BackupType, DeserializationStrategy (+10 more)

### Community 16 - "Message Notification Context"
Cohesion: 0.10
Nodes (18): Boolean, Context, String, Boolean, Context, Int, Message, String (+10 more)

### Community 17 - "Broadcast Receivers (SMS Actions)"
Cohesion: 0.09
Nodes (17): Context, Intent, Context, Intent, Context, Intent, Context, Intent (+9 more)

### Community 18 - "Archived/RecycleBin Conversation Adapters"
Cohesion: 0.11
Nodes (10): ArchivedConversationsAdapter, RecycleBinConversationsAdapter, Conversation, Int, List, Menu, Conversation, Int (+2 more)

### Community 19 - "Conversations Adapter"
Cohesion: 0.14
Nodes (5): ConversationsAdapter, Boolean, Conversation, Int, Menu

### Community 20 - "JSON Object Extensions"
Cohesion: 0.19
Nodes (24): JsonElement, JsonObject, String, optBigDecimal(), optBigInteger(), optBoolean(), optByte(), optCharacter() (+16 more)

### Community 21 - "MMS Sent Receiver"
Cohesion: 0.13
Nodes (14): Context, Int, Intent, Context, Int, Intent, Context, Int (+6 more)

### Community 22 - "Archived Conversations Screen"
Cohesion: 0.15
Nodes (9): ArchivedConversationsActivity, Any, ArrayList, Boolean, Bundle, Conversation, EventBus, Events (+1 more)

### Community 23 - "Recycle Bin Conversations Screen"
Cohesion: 0.15
Nodes (9): RecycleBinConversationsActivity, Any, ArrayList, Boolean, Bundle, Conversation, EventBus, Events (+1 more)

### Community 24 - "Conversation/MMS Query Extensions"
Cohesion: 0.19
Nodes (22): ArrayList, HashMap, Int, Map, Message, SimpleContact, getConversations(), getDefaultKeyboardHeight() (+14 more)

### Community 25 - "Conversations DAO"
Cohesion: 0.19
Nodes (6): Conversation, List, Long, String, ConversationWithSnippetOverride, ConversationsDao

### Community 26 - "Thread Participants Setup"
Cohesion: 0.17
Nodes (4): ArrayList, SimpleContact, View, SIMCard

### Community 27 - "Base Conversations Adapter"
Cohesion: 0.15
Nodes (8): BaseConversationsAdapter, Int, ViewGroup, ViewHolder, Conversation Management, MyRecyclerViewListAdapter, Parcelable, RecyclerViewFastScroller

### Community 28 - "Room Database Definition"
Cohesion: 0.12
Nodes (12): Context, AttachmentsDao, ConversationsDao, getInstance(), MessagesDatabase, migrate(), DraftsDao, MessageAttachmentsDao (+4 more)

### Community 29 - "MMS/SMS Backup Writer"
Cohesion: 0.24
Nodes (7): Boolean, Long, MmsAddress, MmsBackup, MmsPart, SmsBackup, MessagesWriter

### Community 30 - "Conversation Details Screen"
Cohesion: 0.15
Nodes (9): ConversationDetailsActivity, ArrayList, Bundle, Conversation, Long, SimpleContact, SimpleContact, conversationsDB conversation store (+1 more)

### Community 31 - "Build Config & Project Metadata"
Cohesion: 0.14
Nodes (13): hasSigningVars(), Boolean, Release Signing Config, traccar Product Flavor, Dependabot Config, Detekt Config, Traccar SMS Gateway README, Fossify Messages (+5 more)

### Community 32 - "Image Compression"
Cohesion: 0.27
Nodes (8): Bitmap, Boolean, File, Int, Long, Uri, BitmapFactory, ImageCompressor

### Community 33 - "Shortcut Helper"
Cohesion: 0.27
Nodes (7): Boolean, Conversation, List, Long, String, ShortcutHelper, ShortcutInfoCompat

### Community 34 - "Message Sending (Thread)"
Cohesion: 0.23
Nodes (6): Int, List, Long, String, SubscriptionInfo, MutableList

### Community 35 - "Cursor→JSON / Gson Deserializer"
Cohesion: 0.19
Nodes (11): JsonObject, Any, JsonElement, Map, String, rowsToJson(), gson, MapDeserializerDoubleAsIntFix (+3 more)

### Community 36 - "Message Models"
Cohesion: 0.16
Nodes (9): Boolean, Int, SimpleContact, areContentsTheSame(), areItemsTheSame(), Message, RecycleBinMessage, SearchResult (+1 more)

### Community 37 - "Attachment Composing (Thread)"
Cohesion: 0.23
Nodes (3): File, Uri, AttachmentsAdapter

### Community 38 - "Scheduled Message UI"
Cohesion: 0.21
Nodes (3): DateTime, Events, Message

### Community 39 - "Attachment Picker Intents"
Cohesion: 0.26
Nodes (3): Array, Attachment, Intent

### Community 40 - "MMS Sender & Notification Extensions"
Cohesion: 0.15
Nodes (14): Bitmap, Set, String, Cursor, getContactFromAddress(), getMessageRecipientAddress(), getMMSSender(), getNameFromAddress() (+6 more)

### Community 41 - "Gateway Foreground Service"
Cohesion: 0.19
Nodes (7): Context, Int, Intent, String, GatewayService, IBinder, Notification

### Community 42 - "MIME Type String Helpers"
Cohesion: 0.26
Nodes (12): Boolean, String, getExtensionFromMimeType(), isAudioMimeType(), isCalendarMimeType(), isGifMimeType(), isImageMimeType(), isPdfMimeType() (+4 more)

### Community 43 - "Room Type Converters"
Cohesion: 0.27
Nodes (6): ArrayList, Attachment, MessageAttachment, SimpleContact, String, Converters

### Community 44 - "SMS Intent Parser"
Cohesion: 0.29
Nodes (7): Array, Intent, String, Uri, SmsIntentParser.parse, SmsIntentParser, Pair

### Community 45 - "Gateway HTTP Server (Jetty)"
Cohesion: 0.26
Nodes (9): Int, String, GatewayServer, handle(), Handler, HttpServletRequest, HttpServletResponse, Request (+1 more)

### Community 46 - "Thread Items Sealed Types"
Cohesion: 0.33
Nodes (8): ThreadItem, subscriptionManagerCompat(), ThreadDateTime, ThreadError, ThreadItem, ThreadSending, ThreadSent, SubscriptionManager

### Community 47 - "Conversation View Binding"
Cohesion: 0.29
Nodes (6): ConversationDiffCallback, Boolean, Conversation, View, DiffUtil, TextView

### Community 48 - "Message Details Dialog"
Cohesion: 0.29
Nodes (5): List, String, SubscriptionInfo, BasePropertiesDialog, MessageDetailsDialog

### Community 49 - "SimpleContact Extensions"
Cohesion: 0.27
Nodes (9): Context, List, String, getAddresses(), getThreadTitle(), loadIcon(), toPerson(), IconCompat (+1 more)

### Community 50 - "Attachment SMIL Parser"
Cohesion: 0.44
Nodes (5): List, String, AttachmentUtils, parseAttachmentNames, XmlPullParser

### Community 51 - "Drafts DAO"
Cohesion: 0.29
Nodes (5): Int, List, Long, Draft, DraftsDao

### Community 52 - "Conversation Models"
Cohesion: 0.27
Nodes (6): Boolean, ArchivedConversation, areContentsTheSame(), areItemsTheSame(), Conversation, ConversationWithSnippetOverride

### Community 53 - "Gateway Config Activity"
Cohesion: 0.27
Nodes (5): Bundle, List, String, GatewayActivity, SharedPreferences

### Community 54 - "VCard Model"
Cohesion: 0.36
Nodes (8): Context, String, VCard, from(), getPropertyTypeString(), VCardPropertyWrapper, VCardWrapper, VCardProperty

### Community 55 - "SMS Status Sent Receiver"
Cohesion: 0.36
Nodes (5): Context, Int, Intent, Long, SmsStatusSentReceiver

### Community 56 - "Gateway SMS Send Flow"
Cohesion: 0.25
Nodes (6): Boolean, Context, Int, String, Gateway SMS send flow, GatewayServiceUtil

### Community 57 - "Activity Launch Extensions"
Cohesion: 0.32
Nodes (7): Long, String, Unit, Uri, dialNumber(), launchConversationDetails(), launchViewIntent()

### Community 58 - "Collections Extensions"
Cohesion: 0.32
Nodes (7): ArrayList, Int, List, T, filterNotInByKey(), indexOfFirstOrNull(), toArrayList()

### Community 59 - "Conversation Persistence Extensions"
Cohesion: 0.25
Nodes (8): ContentValues, Conversation, toContentValues(), createTemporaryThread(), insertOrUpdateConversation(), renameConversation(), updateLastConversationMessage(), Iterable

### Community 60 - "Attachment Selection Model"
Cohesion: 0.36
Nodes (7): Boolean, Int, String, areContentsTheSame(), areItemsTheSame(), AttachmentSelection, getViewTypeForMimeType()

### Community 62 - "Scheduled Message Alarms"
Cohesion: 0.38
Nodes (6): Long, Message, cancelScheduleSendPendingIntent(), getScheduleSendPendingIntent(), scheduleMessage(), PendingIntent

### Community 65 - "App Class & Messaging Cache"
Cohesion: 0.33
Nodes (3): FossifyApp, MessagingCache, App

### Community 66 - "Adapter RecyclerView State"
Cohesion: 0.60
Nodes (3): onChanged(), onItemRangeInserted(), onItemRangeMoved()

### Community 67 - "Drafts Extensions"
Cohesion: 0.50
Nodes (3): HashMap, Long, String

### Community 68 - "URI File Extensions"
Cohesion: 0.40
Nodes (5): Array, Uri, copyToUri(), getFileSizeFromUri(), queryCursorUnsafe()

### Community 69 - "Attachments DAO"
Cohesion: 0.40
Nodes (3): Attachment, List, AttachmentsDao

### Community 70 - "Message Attachments DAO"
Cohesion: 0.40
Nodes (3): List, MessageAttachment, MessageAttachmentsDao

### Community 71 - "Gateway FCM Service"
Cohesion: 0.40
Nodes (3): FirebaseMessagingService, GatewayMessagingService, RemoteMessage

### Community 75 - "Event Bus Events"
Cohesion: 0.50
Nodes (3): Events, RefreshConversations, RefreshMessages

## Knowledge Gaps
- **278 isolated node(s):** `Boolean`, `EventBus`, `Bundle`, `ArchivedConversationsAdapter`, `Boolean` (+273 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **17 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `ThreadActivity` connect `Thread (Conversation) Screen` to `Main Conversations Screen`, `Message Sending (Thread)`, `Attachment Composing (Thread)`, `Scheduled Message UI`, `Attachment Picker Intents`, `New Conversation Screen`, `Rename Conversation Dialog`, `Settings Screen`, `Event Bus Events`, `Recycle Bin & Deletion Extensions`, `Thread Items Sealed Types`, `Archived Conversations Screen`, `Recycle Bin Conversations Screen`, `Thread Participants Setup`, `Thread Message Loading`, `Conversation Details Screen`, `SimpleActivity Base`?**
  _High betweenness centrality (0.281) - this node is a cross-community bridge._
- **Why does `MainActivity` connect `Main Conversations Screen` to `New Conversation Screen`, `Settings Screen`, `Thread (Conversation) Screen`, `Event Bus Events`, `Archived Conversations Screen`, `Recycle Bin Conversations Screen`, `Conversation Details Screen`, `SimpleActivity Base`?**
  _High betweenness centrality (0.164) - this node is a cross-community bridge._
- **Why does `SimpleActivity` connect `SimpleActivity Base` to `Blocked Keywords Management`, `Main Conversations Screen`, `New Conversation Screen`, `Settings Screen`, `Thread (Conversation) Screen`, `VCard Viewer Screen`, `Gateway Config Activity`, `Archived Conversations Screen`, `Recycle Bin Conversations Screen`, `Conversation Details Screen`?**
  _High betweenness centrality (0.147) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `ThreadActivity` (e.g. with `conversationsDB conversation store` and `app Config preferences`) actually correct?**
  _`ThreadActivity` has 2 INFERRED edges - model-reasoned connections that need verification._
- **Are the 2 inferred relationships involving `MainActivity` (e.g. with `conversationsDB conversation store` and `app Config preferences`) actually correct?**
  _`MainActivity` has 2 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Boolean`, `EventBus`, `Bundle` to the rest of the system?**
  _279 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Thread & Autocomplete Adapters` be split into smaller, more focused modules?**
  _Cohesion score 0.050616050616050616 - nodes in this community are weakly interconnected._