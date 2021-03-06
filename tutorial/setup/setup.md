# How to setup Unity and Vuforia

## MacOS

### Install [Unity 3D](https://unity3d.com/)

    brew cask install unity

### Launch Unity

    open /Applications/Unity/Unity.app

### Sign in (or skip it)

  ![Unity Sign in screenshot](screenshots/1_signin.png)

### Create new project

  ![Unity new project screenshot](screenshots/2_new-project.png)
  ![Unity create project screenshot](screenshots/3_create-project.png)

### Install [Vuforia](https://www.vuforia.com/)

1. Download Vuforia installer

    Edit > Project Settings > Player

    ![Download Vuforia installer screenshot](screenshots/4_find-vuforia-installer.png)

2. Finish Vuforia installer

    ![Vuforia installer screenshot](screenshots/5_vuforia-installer.png)

3. Restart Unity

### Install mobile development tools

Either (for iOS apps)

#### Install Xcode from [App Store](https://itunes.apple.com/gb/app/xcode/id497799835?mt=12)

  1. Open Xcode

    open /Applications/Xcode.app

  2. Add Apple ID to Xcode

      Xcode > Preferences > Accounts

      ![Add Apple ID screenshot](screenshots/7_add-apple-id.png)
      ![Add Apple ID 2 screenshot](screenshots/8_add-apple-id.png)
      ![Sign in Apple ID screenshot](screenshots/9_sign-in-apple-id.png)

Or (for Android apps)

#### Install JDK and Android Studio

1. Install [JDK](https://www.oracle.com/technetwork/java/javase/downloads/index.html)


2. Install [Android Studio](https://developer.android.com/studio/#downloads). Follow the installation wizard and install any SDK packages it recommends.

3. Setup JDK and Android SDK paths in Unity. (Unity > Preferences > External tools)

  ![Setup paths in Unity](screenshots/10_setup-paths.png)