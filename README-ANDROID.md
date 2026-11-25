# FieldLab — Android APK project

This is a native Android WebView wrapper around the same FieldLab app. It bundles the app locally, so the APK does not need a hosted website or an internet connection to run.

## Build an APK with Android Studio
1. Install Android Studio on a Windows, macOS, or Linux computer.
2. Install Android SDK Platform 35 and a compatible Android SDK Build-Tools version using SDK Manager.
3. Open this `FieldLabAndroid` folder in Android Studio.
4. Allow Gradle sync to complete. Use JDK 17 (Android Studio's bundled JBR is suitable).
5. Select **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
6. Android Studio will show the output location. Usually it is `app/build/outputs/apk/debug/app-debug.apk`.
7. Transfer that APK to your Android phone, tap it, and allow installation from that source if Android asks.

## Notes
- This folder is the Android Studio project source, not a precompiled APK.
- The APK must be compiled with Android SDK / Android build tools. Those are not installed in the file-generation environment used to prepare this project.
- For a shareable release APK, use **Build → Generate Signed Bundle / APK** and create a signing key. Keep that key safe for future app updates.
