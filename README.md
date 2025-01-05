# Uncommon Expo CLI Android Build Errors and Solutions

This repository demonstrates solutions to uncommon errors encountered when building Android apps with the Expo CLI.  These errors often go beyond typical Gradle sync issues and involve deeper problems with the Android environment or SDK setup.

## Common Scenarios

* **Gradle version conflicts:** Expo relies on specific Gradle versions. Mismatches can lead to cryptic errors.
* **Android SDK issues:** Problems with the Android SDK installation, missing components, or incorrect paths can cause failures.
* **Environment variables:**  Incorrectly set or missing environment variables can prevent the build process from functioning correctly.
* **Plugin conflicts:** Third-party plugins may clash with Expo's build system.

## Troubleshooting Steps

1. **Verify Android Studio Installation:** Ensure Android Studio is installed correctly and all necessary components (SDKs, build tools, etc.) are up-to-date.
2. **Check Gradle Version:**  Match the Gradle version specified in Expo's documentation for your project.
3. **Clean and Rebuild:**  Use the `expo prebuild` and then `expo build:android` commands to thoroughly clean the project before building again.
4. **Environment Variables:** Check that `ANDROID_HOME` and other relevant environment variables are set correctly.
5. **Examine the Log:** Pay close attention to the complete error message. Often, these logs provide valuable clues about the root cause.
6. **Check for Plugin Conflicts:** If you're using third-party plugins, try temporarily disabling them to see if they are contributing to the issue.
7. **Invalidate Caches/Restart:** In Android Studio, try invalidating caches and restarting.

This repo provides code examples to help illustrate some specific scenarios and their solutions.