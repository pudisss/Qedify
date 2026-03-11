# Qedify - Project Setup Guide

## Prerequisites

Make sure you have the following installed on your machine:

- **Node.js** (v18 or later) — [https://nodejs.org](https://nodejs.org)
- **Git** — [https://git-scm.com](https://git-scm.com)
- **Expo CLI** — installed globally via npm:
  ```bash
  npm install -g expo-cli
  ```
- **Expo Go** app on your phone (available on the App Store / Google Play) — for running the app on a physical device

## Clone the Repository

```bash
git clone https://github.com/pudisss/Qedify.git
cd Qedify
```

## Install Dependencies

```bash
npm install
```

## Run the App

Start the Expo development server:

```bash
npx expo start
```

This will open the Expo DevTools in your terminal. From there you can:

- **Scan the QR code** with Expo Go (Android) or the Camera app (iOS) to run on your phone
- Press **`a`** to open on an Android emulator
- Press **`i`** to open on an iOS simulator (macOS only)
- Press **`w`** to open in a web browser

## Available Scripts

| Command           | Description                   |
| ----------------- | ----------------------------- |
| `npm start`       | Start the Expo dev server     |
| `npm run android` | Start and open on Android     |
| `npm run ios`     | Start and open on iOS         |
| `npm run web`     | Start and open in web browser |
| `npm run lint`    | Run ESLint                    |

## Project Structure

```
app/             → App screens & navigation (Expo Router file-based routing)
  (tabs)/        → Bottom tab screens (Home, Chapters, Ranks, Profile)
components/      → Reusable UI components
constants/       → Theme and config constants
hooks/           → Custom React hooks
assets/images/   → Static image assets
```

## Troubleshooting

- **Metro bundler issues:** Try clearing the cache with `npx expo start -c`
- **Dependency issues:** Delete `node_modules` and `package-lock.json`, then run `npm install` again
- **Expo Go version mismatch:** Make sure your Expo Go app is updated to the latest version
