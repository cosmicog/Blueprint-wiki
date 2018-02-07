Navigate to `app/src/main/res/values/`

* wallpapers.xml

This file contains a string-array and a string:
```xml
<string-array name="wallpapers">
	<item>circles_wall</item>
</string-array>

<string name="default_wallpaper">circles_wall</string>
```

Keep the string-array and string names ("wallpapers" and "default_wallpaper" respectively) exactly as that, for they to be properly recognized.

The items of the array, and the default wallpaper, must match the name of pictures you must add in the folder `app/src/main/res/drawable-nodpi`
