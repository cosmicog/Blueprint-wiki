Navigate to `strings.xml`, located in `res/values/strings.xml`. There are just a couple of necessary changes here, and all of them are explained in comments. Here is the part you'll need to edit:

```xml
<resources>
    <!-- Your app name -->
    <string name="app_name">Blueprint</string>

    <!--    This one applies for Muzei too. Try not to exceed a tweet length (140 characters) -->
    <string name="app_description">A great wallpapers app with hundreds of cool pictures.</string>

    <!--    TODO: Change this link -->
    <!--    This is the link for the JSON file where you have listed your wallpapers -->
    <string name="json_url">https://jahirfiquitiva.me/frames/wallpapers.json</string>

    <!--    Default wallpapers download folder. Always write it like '%1$s/xxxxxxx' -->
    <string name="default_download_folder">%1$s/Frames/Wallpapers</string>
</resources>
````