You can modify the dashboard’s colors in the `colors.xml` file, which you will find under `app/src/main/res/values/colors.xml`. Here is the part that you'll need to modify:

```xml
<resources>
    <!-- Color for Notifications -->
    <color name="notification_color">@color/light_theme_accent</color>

    <!-- Color for Muzei -->
    <color name="muzei_color">@color/light_theme_accent</color>

    <!-- Light Theme -->
    <color name="light_theme_primary_dark">#e0e0e0</color>
    <color name="light_theme_primary">#f5f5f5</color>
    <color name="light_theme_accent">#4285f4</color>
    <color name="light_theme_background">#fafafa</color>
    <color name="light_theme_card_background">#ffffff</color>
    <color name="light_theme_snackbar">@color/light_theme_card_background</color>
    <color name="light_theme_dialogs_button_color">@color/light_theme_accent</color>
    <color name="splash_light_status_bar">@color/light_theme_primary_dark</color>

    <!-- Dark Theme -->
    <color name="dark_theme_primary_dark">#000000</color>
    <color name="dark_theme_primary">#212121</color>
    <color name="dark_theme_accent">#00b0ff</color>
    <color name="dark_theme_background">#303030</color>
    <color name="dark_theme_card_background">#424242</color>
    <color name="dark_theme_snackbar">@color/dark_theme_card_background</color>
    <color name="dark_theme_dialogs_button_color">@color/dark_theme_accent</color>
    <color name="splash_dark_status_bar">@color/dark_theme_primary_dark</color>
</resources>
````

The file is divided into four sections - the notification accent color, the Muzei accent color, the light theme colors and the dark theme colors.

You can modify each value by replacing the text between the “>” and “<” signs with a hexadecimal color code.

The colors' names are pretty self-explanatory, so you should be able to figure out which parts of the dashboard particular values correspond to.

To avoid copying the same color into many fields, you can connect certain values, like the notification accent color, to different values, like the light theme accent color, like so:

```xml
<color name="notification_color">@color/light_theme_accent</color>
````

Remember to edit all the values in this file, to maintain a consistent look throughout all the available dashboard themes.

## Changing the Color of the Filter Chips

To modify the shades of the colored backgrounds behind the filter name entries located in the icon preview section's slide-out filtering drawer, enter custom hexadecimal color codes in each of the following string array's items.

```xml
    <!-- FILTERS COLORS -->
    <!-- Used Material Design 100 shade values -->
    <string-array name="filters_colors">
        <item>#ffcdd2</item>
        <item>#e1bee7</item>
        <item>#c5cae9</item>
        <item>#b3e5fc</item>
        <item>#b2dfdb</item>
        <item>#dcedc8</item>
        <item>#fff9c4</item>
        <item>#ffe0b2</item>
        <item>#d7ccc8</item>
        <item>#cfd8dc</item>
        <item>#f8bbd0</item>
        <item>#d1c4e9</item>
        <item>#bbdefb</item>
        <item>#b2ebf2</item>
        <item>#c8e6c9</item>
        <item>#f0f4c3</item>
        <item>#ffecb3</item>
        <item>#ffccbc</item>
    </string-array>
```