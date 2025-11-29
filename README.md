# essential-signal
Project Codename: Cactus-Hackathon

couldn’t fit into github repo, here’s the wetransfer: https://we.tl/t-3DwAnYk6Md

Build Type: Release (APK Included)

Essential Signal is a local-first, context-aware communication aid designed with a raw "Nothing/Essential" industrial aesthetic. It leverages on-device AI to help neurodivergent users Refine (rewrite drafts) or Decode (analyze sentiment) based on the current screen context.

🛠️ Technical Dependencies

If building from source, ensure the following are installed:

Runtime: Node.js (v18+) & npm

Framework: React Native 0.76+ (New Architecture / Fabric Enabled)

Language: TypeScript, Java (Android Native Modules)

AI Engine: CactusLM (react-native-nitro-modules)

Model: Qwen3-0.6B (Downloaded in-app)

Android SDK: API Level 35 (Minimum SDK 26)

📲 Installation Guide (For Testers)

An optimized Release APK is included in this repository.

Location: ./app-release.apk (Root directory)

Method: Transfer this file to your Android device via USB, Google Drive, or WhatsApp, and tap to install.

Note: Since this is a side-loaded app (not from Play Store), you may see a "Unsafe App" warning. This is normal for development builds. Click "More Details" -> "Install Anyway".

⚙️ Initial Setup (Critical)

Because this app reads screen context to help you reply, it requires Accessibility Permissions. Android 13+ restricts these permissions for side-loaded apps by default. You must follow these steps exactly:

1. Enable Restricted Settings

Long-press the Essential Signal app icon on your home screen.

Tap the (i) Info button to open App Info.

Tap the 3 Dots in the top-right corner.

Select "Allow Restricted Settings".

If you verify your identity (fingerprint/pin), the setting is now unlocked.

2. Grant Accessibility

Open your phone Settings -> Accessibility.

Find "Essential Signal" in the "Downloaded Apps" section.

Toggle the switch ON.

Allow the permission "View and control screen" (Required for context reading).

3. Setup the Signal Tile

Swipe down twice from the top of your screen to open the Quick Settings Panel.

Tap the Pencil (Edit) icon.

Scroll down to find the SIGNAL [ • ] tile.

Drag and drop it to the very top of your active tiles list.

🚀 Usage Guide

Phase 1: First Run (Model Download)

Tap the SIGNAL tile in your Quick Settings.

The app will open. You will see a "SYSTEM_ERR" or "CORE MISSING" alert, or it will take you to Settings.

In the app Settings, tap [ INSTALL ].

Wait for the boot sequence to finish downloading the Qwen3 Brain (approx 400MB).

Once "ACTIVE", tap SAVE & EXIT.

Phase 2: The Workflow (Example)

Scenario: You are reading a confusing Reddit thread or a tense WhatsApp chat.

Open the App: Navigate to the Reddit thread/WhatsApp chat you want help with.

Trigger Signal: Swipe down and tap the SIGNAL tile.

The Notification shade will close automatically.

Wait 1 second. (The app waits for the screen to clear before scanning).

Signal Acquired: You will see a "SIGNAL_ACQUIRED" toast message.

Phase 3: Modes

The interface has two mutually exclusive modes depending on your input:

Mode A: DECODE (Sentiment Analysis)

Action: Leave the text box EMPTY.

Button: The DECODE button will light up.

Result: The AI reads the screen context and tells you the "Vibe" (Semantic Analysis) and suggests a quick reply.

Mode B: REFINE (Rewriting)

Action: Type a rough, messy, or angry draft into the text box.

Button: The REFINE button will light up (Decode turns off).

Result: The AI rewrites your text to be "Clear and Kind" while keeping the context in mind.

⚠️ Troubleshooting

"I tapped the tile but it didn't scan."

Ensure you allowed the Accessibility Permission.

Ensure you waited the split second for the notification shade to close.

"I can't turn on Accessibility."

You missed the "Allow Restricted Settings" step. Go back to App Info -> 3 Dots -> Allow Restricted
