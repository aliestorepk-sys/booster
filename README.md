# Boost App

Android WebView app that loads **https://myboost-co.vercel.app**

## GitHub Actions — Automatic APK Build

Push to `main` ya `master` branch par har push par GitHub Actions automatically APK build karega.

Built APK **Artifacts** me available hogi (30 din tak retain).

### Manual Build
GitHub repo → **Actions** tab → **Boost APK Build** → **Run workflow**

## Project Structure

```
Boost/
├── app/
│   ├── build.gradle
│   ├── proguard-rules.pro
│   └── src/main/
│       ├── AndroidManifest.xml
│       └── java/com/boost/app/
│           └── MainActivity.java
├── build.gradle
├── settings.gradle
├── gradle.properties
└── .github/workflows/build.yml
```

## Features
- WebView with JavaScript enabled
- Back button navigation support
- Cleartext traffic allowed (HTTPS bhi, HTTP bhi)
- Release build with ProGuard minification