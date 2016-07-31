# Setup React Native on OSX

## References
- Youtube: [Setup React Native for Android & iOS Development](https://www.youtube.com/watch?v=iLgJreGpfyM)
- [facebook.github.io](https://facebook.github.io/react-native/docs/getting-started.html)
- [Android Setup](http://facebook.github.io/react-native/releases/0.23/docs/android-setup.html)

## Prerequisites
- Install `Xcode`
- Install [brew](http://brew.sh/)
- Install [nodejs](https://nodejs.org/en/)
  - If you want to use `nvm` (Node Version Manager), instruction can be found [here](https://github.com/tow02/install-nvm-osx)
- Install [Virtualbox](https://www.virtualbox.org/)
  - You might also need to install `VirtualBox Extension Pack`

## Setup
> brew install watchman
> <br/> npm install -g react-native-cli


### Android
- If you already had `Android Studio` or `Android SDK` installed on your computer, uninstall them first. Instruction to remove them all is [here](http://goo.gl/04h8Or).


- Install `JDK`
  - Open Terminal and type `javac`. There will be a popup. Click on `More info` button. It will redirect you to JDK downloading page.

<br/>

- Install `Android SDK`
  > brew install android-sdk


- Add this to `~/.bashrc`, `~/.bash_profile` or whatever shell you use.
  > export ANDROID_HOME=/usr/local/opt/android-sdk

  Then quit Terminal and then re-open it again.


- Configure SDK
  - Run `android` in Terminal and see [this](http://facebook.github.io/react-native/releases/0.23/docs/android-setup.html#configure-your-sdk) for more details


- Install [Genymotion](https://www.genymotion.com/)
  - Go to **Settings** -> **ADB** tab. Click on `Use custom Android SDK tools` and add `/usr/local/opt/android-sdk` to Android SDK
  - Create a virtual device


## Verify Installation
> react-native init demoApp
> <br/> cd demoApp
> <br/> npm start

### Android

Start a virtual device on Genymotion

Open a new tab of Terminal and run
> react-native run-android


### iOS

Open a new tab of Terminal and run
> open ios/demoApp.xcodeproj

Then click run on Xcode

Now you can start develop application for both Android and iOS
