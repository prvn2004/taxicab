## Prerequisites

* **Node.js and npm**: Ensure you have Node.js and npm installed on your system. You can download Node.js from [https://nodejs.org/](https://nodejs.org/).
* **Expo CLI**: Install the Expo CLI using npm:

   ```bash
   npm install -g expo-cli
   ```
* **Expo Account**: Create a free account on Expo by visiting [https://expo.dev](https://expo.dev).
* **EAS CLI**: Ensure you've installed the EAS CLI using npm:

   ```bash
   npm install -g eas-cli
   ```
* **Existing Expo Project**: You need an Expo project to create an APK file.

## Steps

1. **Log in to your Expo Account**:  Use the following command to log in using EAS CLI. If you're already logged in, you can skip this step.

   ```bash
   eas login
   ```
2. **Configure your Project**:
   Use the following command to configure your iOS and/or Android project to be compatible with EAS Build. This process creates a `eas.json` file.

   ```bash
   eas build:configure
   ```
3. **Select Platforms**:
   The command prompt will ask you which platforms you want to configure. Choose "Android" or "All" for Android.

   ```bash
   eas build:configure 
   ```
   *  Choose "All" if you want to configure for both Android and iOS.
   * Choose "Android" if you only want to configure for Android.
4. **Build your APK**:
    Finally, use this command to build your APK file. 
    
    * Replace `your-project-name` with the actual name of your project.
    * Replace `preview` with `production` for deploying to the Play Store.
    
    ```bash
    eas build -p android --profile preview
    ```

## References

* **EAS Build Documentation**: [https://docs.expo.dev/eas/build/](https://docs.expo.dev/eas/build/)
* **Expo Documentation**: [https://docs.expo.dev/](https://docs.expo.dev/)
