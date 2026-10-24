# MediDesk APK

## Easiest: build in the cloud (no Android Studio)
1. Create a free account at github.com and make a new repository.
2. Upload every file in this folder (keep the .github folder).
3. Open the Actions tab, pick "Build APK", then Run workflow.
4. After about 5 minutes, open the finished run and download "MediDesk-APK".
5. Unzip it, send app-debug.apk to your phone, open it and allow "Install unknown apps".

## Or build locally
Needs Node 20, Java 17 and Android Studio.
    npm install
    npx cap add android
    npx cap sync android
    npx cap open android   (then Build > Build APK)
Add the CAMERA permission to android/app/src/main/AndroidManifest.xml for scanning.

## Update the app
Replace www/index.html and build again.
