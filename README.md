# REACT NETIVE Base Template 🚀

**A polished React Native + TypeScript starter template focused on productivity and best practices.**

This repository provides a clean, well-organized foundation for building cross-platform React Native apps with TypeScript, Redux, React Navigation, and common utilities pre-configured.

---

## 🔧 Key Features

- TypeScript-ready project structure
- React Navigation (stack, drawer, bottom tabs)
- Redux with `@reduxjs/toolkit`, `redux-thunk` and `redux-persist`
- Axios configured for API calls
- Reusable UI components (`Button`, `Card`, `Loader`, etc.)
- Theming, colors, and fonts support
- Jest testing scaffolded
- ESLint + Prettier for code quality

---

## 🧩 Quick Start

Prerequisites:
- Node.js >= 18
- Yarn (or npm)
- Android SDK (for Android) / Xcode (for iOS)
- (macOS only) CocoaPods for iOS: `sudo gem install cocoapods`

Install dependencies:

```bash
# Using yarn
yarn install

# or npm
npm install
```

iOS setup (macOS):

```bash
cd ios
pod install
cd ..
```

Run the Metro bundler and app:

```bash
# Start Metro
yarn start

# Run on Android (device/emulator)
yarn android

# Run on iOS (macOS)
yarn ios
```

Test and lint:

```bash
yarn test
yarn lint
```

---

## 🗂 Project Structure (overview)

Top-level notable folders/files:

- `App.tsx` - app entrypoint
- `app/` - main application source
  - `components/` - reusable component library
  - `screens/` - app screens grouped by feature
  - `navigation/` - navigation stacks and navigators
  - `redux/` - store, reducers, persist config, hooks
  - `config/` - Axios and other app-level configs
  - `constants/` - colors, fonts, image paths
  - `assets/` - fonts & images used across the app
- `jest.config.js`, `tsconfig.json`, `babel.config.js` - tooling configuration
- `react-native.config.js` - native linking and asset config

> Tip: The structure is intentionally modular to make adding features and tests straightforward.

---

## 🔁 State Management

This template uses `@reduxjs/toolkit` + `redux-thunk` and persists state using `redux-persist`. See `app/redux/store` and `app/redux/store/persistConfig.ts` for configuration details.

---

## 📡 Networking

API calls are centralized with Axios in `app/config/AxiosConfig.ts`. You can add base URLs and interceptors here for authentication, logging, and error handling.

---

## 🧪 Testing

This template includes Jest and `react-test-renderer`. Tests live under `__tests__/`. Run tests with `yarn test`.

---

## 🛠 Common Tasks / Scripts

- `yarn start` - Start Metro bundler
- `yarn android` - Run app on Android
- `yarn ios` - Run app on iOS (macOS)
- `yarn test` - Run Jest tests
- `yarn lint` - Run ESLint across the project

---

## ✍️ How to Add a Screen

1. Create a folder in `app/screens/<feature>/screens/` and add your screen component.
2. Register the new screen in the appropriate navigator inside `app/navigation/StackNavigators/`.
3. Add styles to the local styles file and tests if needed.

---

## 🎨 Adding Fonts or Images

- Add font files in `app/assets/fonts` and declare them in `react-native.config.js` (already present in this template).
- Run the appropriate native linking step if needed (modern RN supports autolinking).

---

## ✅ Contribution

Contributions are welcome. Please open an issue first for major changes and submit pull requests for fixes, features or documentation improvements. Keep code style consistent with existing patterns and update tests when applicable.

---

## 📄 License

MIT — feel free to reuse and adapt this template for your projects.

---

## 👤 Maintainer

- Maintainer: **@MadhusudanGhule**

---

If you want a customized README (e.g., a shorter version, CI badges, or specific setup for a CI provider), tell me which parts to emphasize and I'll update it. ✅

