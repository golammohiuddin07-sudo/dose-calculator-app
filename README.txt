Dose Calculator v1.2 - Features:
- Expanded presets (adult + pediatric)
- Save / Edit / Delete custom presets (stored in SharedPreferences as JSON)
- Mode switch mg/kg vs mg per unit
- Unit strength handling and units calculation
- GitHub Actions workflow included to build unsigned release APK automatically (see .github/workflows/android-build.yml)
- How to build locally:
  1) Unzip project and open in Android Studio.
  2) Let Gradle sync (may download dependencies).
  3) To build debug APK (auto-signed): Build -> Build Bundle(s) / APK(s) -> Build APK(s).
     OR from command line: ./gradlew assembleDebug
  4) To build unsigned release APK: ./gradlew assembleRelease
     The unsigned release APK will be at app/build/outputs/apk/release/app-release-unsigned.apk
  5) To sign the release APK for Play Store, use Build -> Generate Signed Bundle / APK in Android Studio with your keystore.

- If you want me to produce a signed APK here, you'd need to provide a keystore and passwords (NOT recommended in public chats). Instead, use GitHub Actions with secrets or sign locally.

