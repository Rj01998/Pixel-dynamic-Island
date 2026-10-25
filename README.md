# Pixel Dynamic Island (prototype)

This archive contains:
- `demo.html`: the interactive HTML simulator you supplied.
- `app/`: a native Android/Kotlin starter project that displays a floating pill overlay and can mirror basic notification title/text after notification access is granted.
- `.github/workflows/build-apk.yml`: a cloud build workflow for producing a debug APK.

## Build the APK with GitHub Actions (no local Android SDK required)
1. Create a new GitHub repository and upload the contents of this folder (not the outer folder itself).
2. Open **Actions** and enable workflows if GitHub asks.
3. Run **Build Pixel Dynamic Island APK** from the workflow, or push a commit.
4. Open the completed workflow run and download the `pixel-dynamic-island-debug-apk` artifact.
5. On your Pixel 10a, download the APK, open it, and allow installation from that source if Android prompts you.

## First launch on Pixel 10a
1. Open Pixel Dynamic Island.
2. Grant **Display over other apps**.
3. Open **Notification access** and enable Pixel Dynamic Island notification access if you want notification mirroring.
4. Return to the app and tap **Start floating island**.
5. Tap the pill to expand/minimize; swipe horizontally to dismiss it.

## Permissions and privacy
- Overlay permission is required to draw the pill above other apps.
- Notification access is optional and can expose notification content from other apps to this app. Only enable it if you are comfortable with that.
- Android may stop background services under battery or system restrictions; restart the overlay from the app if it disappears.

## Current limitations
This is a functional starter/prototype, not a feature-complete commercial Dynamic Island replacement. It mirrors basic notification text but does not yet provide guaranteed Maps turn extraction, live cricket data, playback controls, Instagram likes, or WhatsApp inline replies. Those require dedicated integrations and device testing. The debug APK is unsigned for Play Store release.
