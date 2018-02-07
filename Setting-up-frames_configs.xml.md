You will find this file in `app/src/main/res/values/frames_configs.xml`.

There are quite a lot of options here, and each section has a comment explaining what you should edit. 

Here is what the main part of the file looks like:


```xml
<resources>

    <!--    Use old format?
    -       If you're coming from the previous Frames, then you will find this useful
    -       True means yes
    -       False means no
    -->
    <bool name="use_old_json_format">true</bool>

    <!-- Do you want notifications to be enabled for all your users?
    -       True means yes
    -       False means no
    -->
    <bool name="notifications_enabled_by_default">true</bool>

    <!--    Configure your own Splash Screen style
    -       Only change the parent. Available Styles:
    -       LightTheme.SplashScreen
    -       DarkTheme.SplashScreen
    -       TransparentTheme.SplashScreen
    -       AmoledTheme.SplashScreen
    -->
    <style name="MySplashScreen" parent="LightTheme.SplashScreen"/>

    <!--    Define the default app theme
    -       0 -> Light
    -       1 -> Dark
    -       2 -> Transparent
    -       3 -> Amoled
    -       4 -> Auto Light-Dark
    -       5 -> Auto Light-Amoled
    -->
    <integer name="default_theme">0</integer>

    <!--    Choose whether you want colored tiles by default -->
    <bool name="enable_colored_tiles">true</bool>

    <!--    Show wallpaper details bottom sheet or dialog
    -       True to show a bottom sheet
    -       False to show a dialog
    -->
    <bool name="show_bottom_sheet">true</bool>

    <!--    These are your donation items. Only put their ids here -->
    <string-array name="donation_items">
        <item>coffee</item>
        <item>pizza</item>
        <item>burger</item>
    </string-array>
</resources>
````