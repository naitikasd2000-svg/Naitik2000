# Case Battery Android wrapper

This project packages the supplied HTML into an Android WebView app and uses GitHub Actions to build a debug APK.

## Build on GitHub using your phone
1. Create a new empty repository on GitHub.
2. Upload all files and folders from this ZIP to the repository, preserving folder structure.
3. Open the repository's Actions tab.
4. Select "Build Case Battery APK" and tap "Run workflow" (or push to main).
5. When the workflow finishes, open the run and scroll to Artifacts.
6. Download CaseBattery-debug-apk, extract that ZIP, then install app-debug.apk on Android.

## Important limitations
This is a WebView wrapper, not a full native rewrite. Android WebView generally does not provide the Web Bluetooth API used by the HTML, so Bluetooth earbud battery reading/pairing may not work inside this APK. Native Bluetooth code would be needed for reliable support. Voice recognition also depends on the device/WebView. This is a debug APK for testing, not a store-ready signed release.
