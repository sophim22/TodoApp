# TodoApp
# Project Setup Instructions

After cloning the repository, follow these steps to set up and run the project:

## 1. Install Dependencies
Run the following command to install all required dependencies:
```bash
npm install
```

## 2. Add Capacitor Platforms
The `android` and `ios` platforms are not included in the repository by default. You need to add them manually:

**Add Android Platform**:
```bash
npx cap add android
```

**Add iOS Platform**:
```bash
npx cap add ios
```

## 3. Sync Capacitor Platforms
Sync the web assets and configuration to the native platforms:
```bash
npx cap sync
```

## 4. Build the Ionic App
Compile the web assets before running on native platforms:
```bash
ionic build
```

## 5. Run on Android Emulator
Ensure you have Android Studio installed. Then, open the Android project and run it on an emulator:
```bash
npx cap open android
```

## 6. Run on iOS Simulator
Ensure you have Xcode installed. Then, open the iOS project and run it on a simulator:
```bash
npx cap open ios
```

## Notes
- Ensure you have the correct versions of Node.js and npm installed.
- For Android development, install Android Studio and set up an emulator.
- For iOS development, install Xcode and set up a simulator.
- Always run `ionic build` and `npx cap sync` after making changes to the web assets or configuration.
