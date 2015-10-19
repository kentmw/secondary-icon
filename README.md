# Secondary Icon Plugin for Android Phonegap Build applications

## DESCRIPTION
Phonegap Build doesn't let you bring in resources into the /res directory making it impossible for developers to utilize the application-specific R class or assign images a resource id. This causes issues especially for push notifications on Lolipop that require the small icon to be white and transparent. This plugin lets you add a secondary icon to the application resources.

Just place your secondary-icon.png's in:
res/drawable-hdpi/secondary-icon.png
res/drawable-mdpi/secondary-icon.png
res/drawable-xhdpi/secondary-icon.png
res/drawable-xxhdpi/secondary-icon.png

The res directory should be at the root directory of the zip you send to PGB.