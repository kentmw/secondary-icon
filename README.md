# Secondary Icon Plugin for Android Phonegap Build applications

**DEPRECATED - in favor of putting assets under the /locales/android/drawables directory. See http://stackoverflow.com/questions/30802589/how-to-add-native-image-with-phonegap-build/33221780#33221780**

## DESCRIPTION
Phonegap Build doesn't let you bring in resources into the /res directory making it impossible for developers to utilize the application-specific R class or assign images a resource id. This causes issues especially for push notifications on Lolipop that require the small icon to be white and transparent.

## IMPORTANT
Because plugins can not reference files in your project inside the plugin.xml, please fork this plugin for your own use and change out the resources in
```
src/android/res/drawable-hdpi/secondary_icon.png
src/android/res/drawable-mdpi/secondary_icon.png
src/android/res/drawable-xhdpi/secondary_icon.png
src/android/res/drawable-xxhdpi/secondary_icon.png
```

You need a push notification plugin that uses:
```
new NotificationCompat.Builder(context)
        .setSmallIcon(context.getResources().getIdentifier("secondary_icon", "drawable", context.getPackageName()))
```
