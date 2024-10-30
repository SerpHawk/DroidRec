<img src="icons_vector/app_icon.svg" alt="DroidRec Icon" width="200"/>

# DroidRec
***An open-source Android screen recorder.***

<img src="metadata/en-US/images/phoneScreenshots/1.jpg" alt="DroidRec Screenshot 1" width="300"/> <img src="metadata/en-US/images/phoneScreenshots/2.jpg" alt="DroidRec Screenshot 2" width="300"/>

*Audio Playback recording requires Android 10 or later. No Root needed*

*(**WARNING**: Some device vendors may not allow recording certain Audio Playback sources, or even recording applications' audio at all)*

> Licensed under [The Unlicense](LICENSE)

[<img src="https://fdroid.gitlab.io/artwork/badge/get-it-on.png"
     alt="Get it on F-Droid"
     height="80">](https://f-droid.org/packages/com.yakovlevegor.DroidRec/)
[<img src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png"
     alt="Get it on Google Play"
     height="80">](https://play.google.com/store/apps/details?id=com.yakovlevegor.DroidRec)

Or download the apk from [the release section](https://github.com/egorolegovichyakovlev/DroidRec/releases)

## Building

To build this app, run:

`gradle assembleRelease`

To sign the build, first generate your keystore file:

`keytool -genkeypair -keystore signature.keystore -validity 365000 -keysize 4096 -keyalg RSA`

The signature file should be named **signature.keystore**

(**Note**: Run `keytool` from the same or older Java version on which you are going to build the application)

Then run **quicksign.bash** to sign the application. If Android SDK isn't defined in your path, specify the location of your `android-sdk/build-tools/VERSION` folder as an argument.

Example:

`./quicksign.bash $ANDROID_HOME/build-tools/34.0.0`

<hr>

English | [עברית](README.he.md)
