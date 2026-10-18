<p align="center">
  <img width="120" src="app/src/main/res/mipmap/ic_launcher.png" />
  <h1 align="center">EteSync - Secure Data Sync</h1>
</p>

Secure, end-to-end encrypted, and privacy respecting sync for your contacts, calendars and tasks (Android client).

> [!NOTE]
> **This is a maintenance fork of [etesync/android](https://github.com/etesync/android)**, which only sees sporadic activity (last commit February 2026).
>
> EteSync is one of the few open-source products that can encrypt both contacts and calendars E2E and sync them between devices. I use it myself, so I keep this fork going for **security fixes, bug fixes and dependency updates only**. New features are out of scope. Fixes are also [submitted upstream as pull requests](https://github.com/etesync/android/pulls?q=is%3Apr+author%3APrivateBasicsApp), where they are still pending. I'm not affiliated with the original authors. The matching server fork is [PrivateBasicsApp/EteSyncServer](https://github.com/PrivateBasicsApp/EteSyncServer).
>
> There are no prebuilt releases: to use this fork, build it from source (see [Building](#building)). The app keeps the same application ID as the official one but is signed with a different key, so Android won't install it over the Google Play or F-Droid version. Sync any pending changes, uninstall the official app, install your build and log in again: your data is restored from the server.

# Overview

Please see the [EteSync website](https://www.etesync.com) for more information.

EteSync is licensed under the [GPLv3 License](LICENSE).

# Building

EteSync uses `git-submodules`, so cloning the code requires slightly different commands.

1. Clone the repo: `git clone --recurse-submodules https://github.com/PrivateBasicsApp/EteSync-Android etesync-android`
2. Change to the directory `cd etesync-android`
3. Open with Android studio or build with gradle:
  1. Android studio (easier): `android-studio .`
  2. Gradle: `./gradlew assembleDebug`
  
To update the code to the latest version, run: `git pull --rebase --recurse-submodules`

# Translating

Translators are highly welcome! 
To help with translation please go to [our Weblate page](https://hosted.weblate.org/projects/etesync/) and translate it from there.


Third Party Code
================

EteSync's source code was originally based on [DAVdroid](https://www.davx5.com) but the codebases has since diverged quite significantly.

This project relies on many great third party libraries. Please take a look at the
app's about menu for more information about them and their licenses.
