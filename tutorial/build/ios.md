# How to build and deploy to iOS

## Install iOS module

1. Download iOS module

    File > Build Settings
    ![Download iOS module screenshot](screenshots/1_download-ios-module.png)

2. Install iOS module
    ![Install iOS module screenshot](screenshots/2_install-ios-module.png)

3. Restart Unity

## Build for iOS

1. Open File > Build Settings
2. Select your scene from "Scenes in Build"
3. Select iOS Platform
4. Click Switch Platform button
5. Open Player Settings
6. Make sure "Vuforia Augmented Reality" is selected
7. Set **unique** "Bundle identifier" in Other Settings
8. Click Build button

![Build for iOS screenshot](screenshots/3_build-for-ios.png)
![Set bundle identifier screenshot](screenshots/4_set-bundle-identifier.png)

## Open in Xcode

File > Open
![Open in Xcode screenshot](screenshots/5_open-in-xcode.png)

Set signing team for target
![Set signing team screenshot](screenshots/6_set-signing-team.png)

## Deploy to device

1. Connect your iOS device to your laptop via USB
2. Deploy app to your device
![Deploy to device screenshot](screenshots/7_deploy-to-device.png)

[More instructions on Unity page](https://unity3d.com/learn/tutorials/topics/mobile-touch/building-your-unity-game-ios-device-testing)
