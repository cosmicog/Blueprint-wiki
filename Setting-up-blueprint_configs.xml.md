You will find this file in `app/src/main/res/values/blueprint_configs.xml`.

There are quite a lot of options here, and each section has a comment explaining what you should edit. 

Here is what the main part of the file looks like:


```xml
<resources>
	<!-- Icon Pack designer/owner e-mail -->
    <string name="email">someone@email.com</string>

    <!-- Mail subjects for simple e-mail and requests e-mail -->
    <string name="email_subject">Blueprint</string>
    <string name="request_title">Blueprint Icon Request</string>

    <!-- This are the strings for the cards in the main screen -->
    <string name="welcome_title">Welcome to Blueprint</string>

    <!-- Strings for Wallpapers and Requests -->
    <string name="request_save_location">%1$s/Blueprint/Requests/</string>

    <!--
        Set a drawable name in case you want to use a static picture for icons preview.
        Leave empty if you don't want to use a static one.
    -->
    <string name="icons_preview_picture"></string>

    <!--
        Do you want the app to read the icons from res/xml/drawable.xml ? (true)
        Or do you prefer the icons to be loaded from res/values/icon_pack.xml ? (false)
    -->
    <bool name="xml_drawable_enabled">false</bool>


    <!--
        Do you want the app name and version in the drawer header?
        True, means yes.
        False, means no.
    -->
    <bool name="with_drawer_texts">true</bool>

    <!--
        Would you like apply section cards to be colored?
        True, means yes.
        False, means no.
    -->
    <bool name="enable_colored_cards">false</bool>

    <!--
    1. Set the max amount of apps to request.
    2. Limit requests to 1 every X minutes.
    Replace X with the number of minutes you want.
    60 means 1 request every 1 hour.
    1440 means 1 request per day.
    10080 means 1 request per week.
    40320 means 1 request per month.

    App Limit:
    If the apps limit is 0, users won't be able to request anything.
    If the apps limit is -1, users can request as many times they want, and
    as many apps they want.

    Time limit:
    If the time limit is set to 0 or less, users will be able to request as many times they want,
    with the max apps limit.
    -->
    <integer name="max_apps_to_request">-1</integer>
    <integer name="time_limit_in_minutes">0</integer>

    <!-- Leave empty to disable. A URL to an Arctic Request Manager server, e.g. https://arcticmanager.com -->
    <string name="arctic_backend_host"></string>

    <!-- Host must also be filled in first. An app API key from Arctic Request Manager. -->
    <string name="arctic_backend_api_key"></string>
</resources>
```