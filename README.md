# mobileapp

This project contains a minimal Kotlin Android app.

To build an APK locally you need Android SDK and a compatible Gradle version (Gradle 7.x for the
Android Gradle Plugin used here). Quick steps:

1. Install Android SDK command-line tools and set `ANDROID_SDK_ROOT`.
2. Install a compatible Gradle (7.6 recommended) or generate the wrapper on a machine with compatible Gradle.
3. From the project root run:

```bash
export ANDROID_SDK_ROOT=~/Android/Sdk
# if you have the gradle wrapper run ./gradlew assembleDebug
# or with a local gradle binary:
gradle assembleDebug

# APK will be at:
ls app/build/outputs/apk/debug/app-debug.apk
```

Alternatively, push to `main` and the included GitHub Actions workflow will build the debug APK and
attach it as a workflow artifact named `app-debug-apk`.
# mobileapp