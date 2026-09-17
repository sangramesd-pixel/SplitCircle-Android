# SplitCircle – Android expense splitter

SplitCircle is a shared Android expense splitter backed by Firebase Cloud Firestore.

## Features

- Register or sign in with email and password
- Create a group or join friends using an 8-character code
- Record an expense, payer, and participating friends
- Split each expense equally among selected participants
- See each friend's running balance
- Generate a simplified "who pays whom" settlement list
- Delete expenses by long-pressing them
- Synchronize the same shared database across friends' phones
- Share the latest app download link from inside the app
- Pick a phone contact and send a ready-made group invitation by message
- Secure each group's data with Firebase Authentication and Firestore rules

## Install

Download the latest signed APK from the [GitHub Releases page](https://github.com/sangramesd-pixel/SplitCircle-Android/releases/latest). On first installation, Android may ask you to allow installs from the browser or file manager you used to download it.

## Contact invitations

Open a group and tap **Invite contact**. Android's contact picker returns only the selected phone number to SplitCircle, so the app does not request permission to read the whole contact list. The message contains the group code and the latest app download link.

## Open and build

1. Extract this project and open the `ExpenseSplitterAndroid` folder in Android Studio.
2. Allow Gradle sync to complete. Use JDK 17 if Android Studio asks.
3. Select **Build > Build APK(s)**.
4. The debug APK will be created at `app/build/outputs/apk/debug/app-debug.apk`.

The project uses Android SDK 35, has no third-party libraries, and supports Android 6.0 and later.
