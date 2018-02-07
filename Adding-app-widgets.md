**These widgets are not related to Zooper nor Kustom**


Check this folder to find the pictures the app uses for the widgets: 

`app/src/main/res/drawable-nodpi/`


**Clock Widget**

This widget requires 3 pictures. Is very important that you keep the same file names, otherwise you will have to edit the `AndroidManifest.xml` file... :


- clock_bg

Is the background of the clock.


- clock_hour_hand

Is the hour hand of the clock. When creating a new one, make sure it points to 12.

- clock_minute_hand

Is the minute hand of the clock. When creating a new one, make sure it points to 12, too.



**Launcher Icon restorer widget**

This widget require just one picture, but it is a .9.png

To get a .9.png:
- Create a 512x512 px version of you app icon.
- Go to [this site](https://romannurik.github.io/AndroidAssetStudio/nine-patches.html)
- Click in "Select image" and select your icon.
- Tap XXHDPI in source density.
- Tap CONTENT PADDING as edit mode.
- Then in drawable name, name it: "app_logo" (without quotes).
- Then press in "Download .zip" button.
- Then extract the icon inside `res/drawable-xxxhdpi`, in `res/drawable/widgets/drawable-nodpi/`

That's it.

**Remember to rebuild your project for the changes to take effect.**