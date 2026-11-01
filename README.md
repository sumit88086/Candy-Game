# Candy — Android Match-3 starter

A native Android Studio starter project for a simple Candy-style match-3 game.

## Included
- 7x7 candy board
- Adjacent candy swapping
- Match-3 horizontal/vertical clearing, gravity and refill
- Score and 25 moves
- Guest play
- Google sign-in integration scaffold using Firebase Authentication

## Open and run
1. Install Android Studio (current stable) and Android SDK 35.
2. Open this folder in Android Studio and let Gradle sync.
3. Run on an Android device/emulator (Android 6.0+).

## Enable Google login
Google login will not work until you configure your own Firebase project:
1. Create a project at https://console.firebase.google.com/
2. Add an Android app with package name `com.example.candy`.
3. Add your SHA-1 and SHA-256 signing certificate fingerprints in Firebase project settings.
4. Enable **Authentication → Sign-in method → Google**.
5. Download `google-services.json` and place it in the `app/` folder.
6. Sync Gradle and run again. The project applies the Google Services Gradle plugin only after the JSON file is present.

Guest play works without Firebase. The starter currently keeps guest progress only for the current game session; persistent save, cloud sync and a proper guest-to-Google account link are not included yet.

## Before Play Store release
- Change `applicationId` and package/namespace to your own unique package.
- Add your own app icon, screenshots, privacy policy and store listing.
- Configure Firebase with the final package name and signing fingerprints.
- Build a signed Android App Bundle (AAB) from **Build → Generate Signed Bundle / APK → Android App Bundle**.
- Test on multiple screen sizes and Android versions.
- Complete Google Play Data safety, content rating and target API requirements.

This is a starter project, not a finished commercial game. It has no ads, in-app purchases, analytics, online leaderboard or backend.
