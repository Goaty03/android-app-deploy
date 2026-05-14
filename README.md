# 🤖 Android App with FREE CI/CD Pipeline

This Android app is automatically built and deployed using **GitHub Actions** - completely FREE!

## 🚀 Features

- ✅ **Automated builds** on every push
- ✅ **APK generation** for testing
- ✅ **AAB generation** for Play Store
- ✅ **Code signing** with secrets
- ✅ **Google Play deployment** (when configured)
- ✅ **Artifact storage** for downloads

## 🏗️ Build Status

![Android CI/CD Pipeline](https://github.com/Goaty03/android-app-deploy/workflows/Android%20CI/CD%20Pipeline/badge.svg)

## 📱 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/Goaty03/android-app-deploy.git
   cd android-app-deploy
   ```

2. Open in Android Studio

3. Build and run:
   ```bash
   ./gradlew assembleDebug
   ```

## 🔐 Setting Up Code Signing

To enable release builds, add these secrets to your GitHub repository:

1. Go to **Settings** → **Secrets and variables** → **Actions**
2. Add these secrets:
   - `SIGNING_KEY_ALIAS` - Your keystore alias
   - `SIGNING_KEY_PASSWORD` - Your key password
   - `SIGNING_STORE_PASSWORD` - Your keystore password

## 🏪 Google Play Store Deployment

To deploy to Google Play Store:

1. Create a service account in Google Play Console
2. Add `PLAY_STORE_SERVICE_ACCOUNT_JSON` secret
3. Update `packageName` in the workflow file

## 🎯 Deployment Targets

- **Debug builds**: Every push to any branch
- **Release builds**: Push to `main` branch
- **Play Store**: Automatic deployment to Internal Testing

## 🆓 FREE Resources Used

- **GitHub Actions**: 2,000 minutes/month (private repos), unlimited (public)
- **GitHub Storage**: Build artifacts stored
- **No additional costs**: Everything runs on GitHub's infrastructure

## 🔄 Workflow Triggers

- Push to `main` or `develop`
- Pull requests to `main`
- Manual trigger via GitHub UI

## 📋 Build Outputs

- **Debug APK**: Available in Actions artifacts
- **Release APK**: Available in Actions artifacts
- **Release AAB**: Deployed to Play Store (if configured)

## 🛠️ Tech Stack

- **Language**: Kotlin
- **Build**: Gradle
- **CI/CD**: GitHub Actions
- **Deployment**: Google Play Console (optional)

## 📞 Support

- Open an issue for bugs
- Fork and contribute improvements
- Star if this helped you! ⭐