Navigate to `app/src/main/res/values/`


There you will find a set of more XMLs, which are required for the icon pack to work properly too.


Those files are:
- bools.xml
- docks.xml
- icon_pack.xml
- skin_colors.xml
- wallpapers.xml


You can keep bools.xml and skin_colors.xml exactly as they are.

---

**How to edit the other files...**

* docks.xml

	This file only contains an array:
	```xml
	<string-array name="dock_backgroundlist">
		<item>dock_a</item>
		<item>dock_b</item>
	</string-array>
	```

	The items must match the names of png pictures you must add in the same folder where the icons go.
	Also, keep the string-array name (dock_backgroundlist) exactly as it is, otherwise this list may not work properly.

	If you don't want to provide docks, simply remove all items from this array.


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


* Now the longest file

	`icon_pack.xml`


	This file contains many arrays that contains the names of the icons files.


	I will try to explain only by the name:
	

	`<string-array name="icons_preview">`
	This array contains the icons names that will be shown in the icons preview. Try to keep at least 8 icons there.

	`<string-array name="icon_filters">`
	This array contains the filters names that will be used in the icons preview section. Make sure the names you put in the array, match the names of the other arrays. I mean, as you see, the next array is named "something", so I will put "something" as an item of the array `icon_filters`.

	`<string-array name="something">`
	You can create more arrays with any name you want. The arrays you create will be taken into account to generate the filters in the icons preview section.

	`<string-array name="icon_pack">`
	This array is needed by some launchers too.

**If you think creating this file is tedious, or a bit hard, you might want to check the [tool Allan Wang created](https://github.com/jahirfiquitiva/IconShowcase-Dashboard/wiki/Tools).**

That's it.