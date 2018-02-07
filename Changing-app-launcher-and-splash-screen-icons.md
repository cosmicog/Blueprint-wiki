## Change splash screen icon
1. Go to `app/src/main/res` folder
2. Create a folder with name `drawable-nodpi`
3. Put your app icon there in **png** format. Optimal dimensions: 288 x 288 pixels.
4. Make sure your icon is named `app_logo.png`

## Change launcher icons
1. Go to `app/src/main/res` folder
2. There you will find some `mipmap-xxxxx` folders
3. Put your icons in every folder with the following sizes:

| **Folder suffix** | **Dimensions** (in pixels) |
|:-----------------:|:--------------------------:|
|        mdpi       |            48x48           |
|        hdpi       |            72x72           |
|       xhdpi       |            96x96           |
|       xxhdpi      |           144x144          |
|      xxxhdpi      |           192x192          |


## Other icons

[**Add rounded icon**](https://developer.android.com/about/versions/nougat/android-7.1.html#circular-icons)

[**Add adaptive icons**](https://developer.android.com/guide/practices/ui_guidelines/icon_design_adaptive.html)