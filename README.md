# Expo Android Build Failure: `android:attr/fontVariationSettings` Not Found

This repository demonstrates a bug encountered while building an Android APK using Expo CLI. The build process fails with a resource linking error, specifically mentioning `android:attr/fontVariationSettings`. This usually points to an incompatibility between the Expo version and the Android Gradle Plugin (AGP) version used in the project.

## Bug Description
The Expo CLI build process fails with an error related to the `android:attr/fontVariationSettings` resource not being found.  This issue is likely due to version conflicts between Expo, the AGP, and potentially the fonts used in the application.

## How to Reproduce
1.  Clone this repository.
2.  Attempt to build an Android APK using `expo build:android`.

## Solution
The solution is to downgrade the Android Gradle Plugin (AGP) to a version that's compatible with the Expo version used.  See the `bugSolution.js` file for details on how this was resolved in this specific case.

## Additional Notes
Always check for updates to both Expo and the Android Gradle Plugin. Make sure both are compatible before starting a build to avoid this issue. Consider using a newer version of Expo that has better AGP compatibility.