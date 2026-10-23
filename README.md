# Jake Pong (Android)

A simple offline ping-pong game for Android. Drag on the left side to move your paddle. First to 7 points wins. The footer credits **jake.wav** and uses the supplied profile image.

## Build an APK
1. Open this folder in Android Studio.
2. Let Gradle sync and install the Android SDK requested by the project.
3. Select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
4. Install the generated APK on your Android device.

No internet permission or network access is required. This is an Android Studio project, not a precompiled APK.

## Build APK in the cloud (no Android SDK on your phone)

This repository includes a GitHub Actions workflow at `.github/workflows/build-apk.yml`.

1. Create a GitHub repository and upload the contents of this project (the files inside `JakePongAndroid`, including the hidden `.github` folder).
2. Open the repository's **Actions** tab and enable Actions if prompted.
3. Run **Build Jake Pong APK** using **Run workflow**, or push to `main`.
4. When the run completes, open it and download the **Jake-Pong-APK** artifact.
5. Extract the downloaded artifact ZIP; it contains `app-debug.apk`.

The build runs on GitHub-hosted cloud runners, not on your phone. The APK is a debug-signed installable build.
