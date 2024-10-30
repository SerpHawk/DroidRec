<img src="icons_vector/app_icon.svg" alt="DroidRec תמונה" width="200"/>

# DroidRec
***רשם מסך אנדרואיד.***

<img src="metadata/en-US/images/phoneScreenshots/1.jpg" alt="DroidRec צילם 1" width="300"/> <img src="metadata/en-US/images/phoneScreenshots/2.jpg" alt="DroidRec צילם 2" width="300"/>

*לרשום שמע יישומים עדכונך אנדרואיד צריך להיות חדש מ-10. אין הכרח רוט*

*(**זהירות**: לא כל יישומים או מכשירים מתירים לרשום שמעיהם)*

> [The Unlicense](LICENSE) תעודה

[<img src="https://fdroid.gitlab.io/artwork/badge/get-it-on.png"
     alt="Get it on F-Droid"
     height="80">](https://f-droid.org/packages/com.yakovlevegor.DroidRec/)
[<img src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png"
     alt="Get it on Google Play"
     height="80">](https://play.google.com/store/apps/details?id=com.yakovlevegor.DroidRec)

[רכש היישום](https://github.com/egorolegovichyakovlev/DroidRec/releases)

## קימפל היישום

במצווה:

`gradle assembleRelease`

אז ברא המפתח:

`keytool -genkeypair -keystore signature.keystore -validity 365000 -keysize 4096 -keyalg RSA`

בשם **signature.keystore**

(**לשם לב**: ג'אוותך עדכון צריך להיות לא חדש מג'אווה אנדרואיד־SDK)

אז תציווה **quicksign.bash** לחתם היישום

אם להגדרותיך אין דרך אנדרואיד־SDK תוסיף דרכו במצווה כך `android-sdk/build-tools/VERSION`

למשל:

`./quicksign.bash $ANDROID_HOME/build-tools/34.0.0`

<hr>

[English](README.md) | עברית
