You will find this file in `app/src/main/res/values/kuper_configs.xml`.

There are quite a lot of options here, and each section has a comment explaining what you should edit. 

Here is what the main part of the file looks like:


```xml
<resources>

    <!--    Set to 'true' if your app requires Kolorette. 'false' otherwise. -->
    <bool name="kolorette_required">false</bool>


    <!--    ZOOPER EXCLUSIVE CONFIGS -->

    <!-- These texts are shown in Zooper -->
    <string name="zooper_pack_name">@string/app_name</string>
    <string name="zooper_pack_desc">Cool widgets.</string>
    <string name="zooper_pack_author">Your name</string>

    <!--    If set to 0, the user will not be allowed to save the templates you provide -->
    <integer name="zooper_pack_allowsave">1</integer>

    <!-- This is the icon that will be shown in Zooper -->
    <drawable name="zooper_pack_icon">@mipmap/ic_launcher</drawable>

    <!--    Set to 'true' if your app requires Media Utils. 'false' otherwise. -->
    <bool name="media_utils_required">false</bool>


    <!--    KUSTOM EXCLUSIVE CONFIGS -->

    <!--    Name of the skin to be shown inside the Kustom app -->
    <string name="kustom_pack_title">@string/app_name</string>

    <!--    A brief description of the pack contents -->
    <string name="kustom_pack_description">Cool Kustom komponents, wallpapers and widgets.</string>
</resources>
````