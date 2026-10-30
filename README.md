# Flash Launcher — Android project starter

This is the first Android Studio source scaffold for Flash Launcher, using a dark purple animated Compose UI and the requested lightning-bolt branding.

## Open
1. Install Android Studio (current stable).
2. Choose **Open** and select this `FlashLauncher` folder.
3. Let Gradle sync.
4. Connect an Android device with USB debugging enabled, or use an emulator.
5. Run the `app` configuration.

## Important status
This is **not yet a playable Minecraft launcher APK**. It is the UI and Android project foundation only. The Play button intentionally displays a status message rather than pretending to launch Minecraft.

A real playable Java launcher still needs:
- A legally compliant Minecraft Java game-file downloader and version manifest.
- A compatible Android Java runtime and native library integration.
- A supported renderer / OpenGL translation layer and input controls.
- Secure Microsoft OAuth authentication and token refresh.
- Ely.by authentication integration according to its current API.
- Offline profile support only for offline-mode servers; it does not grant access to authenticated servers.
- Per-version compatibility checks, mod-loader installation, storage permissions and crash handling.

Minecraft 26.3 and historical versions must be verified against official manifests and the chosen runtime. Not every version, mod loader, shader or mod will work on Android.

Package ID: `com.flashlauncher`
App version: `0.1.0`

## Build an APK using only an Android phone

1. In Chrome, open https://github.com and sign in or create an account.
2. Create a new repository named `FlashLauncher` (Public or Private).
3. On the new repository page, choose **Add file → Upload files**.
4. Extract this ZIP on your phone first. Upload the contents of the extracted `FlashLauncher` folder, including the hidden `.github` folder. If your file manager hides dot-folders, enable **Show hidden files**.
5. Commit the uploaded files to the `main` branch.
6. Open the repository's **Actions** tab. Approve/enable workflows if GitHub asks.
7. Open **Build Flash Launcher APK** and tap **Run workflow** if it has not started automatically.
8. Wait for the run to finish successfully. Open the completed run and find **Artifacts** at the bottom.
9. Download `Flash-Launcher-debug-apk`, extract it, then tap `app-debug.apk` to install. Android may ask you to allow installs from that browser/file manager; only allow it for this APK if you trust the source.

This workflow builds the current starter UI as a debug APK. It does not add the Minecraft Java runtime, game downloads, Microsoft/Ely.by authentication, or real mod/shader installation. The Play button remains a placeholder until those systems are integrated.
