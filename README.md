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

## Setup

> brew install watchman <br/> npm install -g react-native-cli


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
