Sala 13 - Android project (WebView)
==================================

What is included:
- Android Studio project skeleton (Kotlin)
- MainActivity loads https://sala-financiar-14332cdf.base44.app/ in a WebView
- App name: Sala 13
- Min SDK: 21 (Android 5.0 Lollipop)
- Simple emblem-style icon (dark background) in res/mipmap-anydpi-v26/ic_launcher.png

Important notes:
- This is a project skeleton ready to be opened in Android Studio (recommended).
- Building an APK requires Android Studio or command-line Android SDK + Gradle.
- I could not run the Android build environment here. You (or your friends) can build the APK locally.

Build instructions (Android Studio):
1. Open Android Studio.
2. Choose 'Open' and pick the folder: Sala13_project (the root).
3. Let Gradle sync. If Android Studio prompts to update Gradle plugin, follow prompts.
4. Build > Build Bundle(s) / APK(s) > Build APK(s).
5. The generated APK will be in app/build/outputs/apk/.

Build instructions (command line, if you have Android SDK & Gradle installed):
1. From project root: ./gradlew assembleDebug   (Linux/macOS)
   or gradlew assembleDebug (Windows)
2. The debug APK will be at app/build/outputs/apk/debug/app-debug.apk

Signing / Distribution:
- For easy sharing between friends (without Play Store), you can share the debug APK
  but Android may require enabling "Install unknown apps" for the recipient.
- For publishing on Play Store, create a release build and sign it with your keystore.

Replacing the icon:
- Swap the PNG files in res/mipmap-* or res/drawable with your preferred assets.

If you want, I can:
- generate higher-quality SVG-based icon variants (you can upload a sketch/reference)
- produce a signed release APK (I can't sign it here without your keystore; you can provide instructions)
- add splash screen or fullscreen immersive mode
