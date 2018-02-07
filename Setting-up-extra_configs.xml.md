You will find this file in `app/src/main/res/values/extra_configs.xml`.

There are quite a lot of options here, and each section has a comment explaining what you should edit. 

Here is what the main part of the file looks like:


```xml
<resources>
	<!-- Launcher Activity Name
    if the activity is:
    com.packagename.appname.Activity
    then write Activity
    -->
    <string name="main_activity_name">MainActivity</string>
    <string name="main_activity_fullname">com.packagename.appname.MainActivity</string>

    <!--    These arrays are for the list of apps or links in main section. -->
    <string-array name="home_list_titles">
		<item>IconShowcase</item>
    </string-array>
    <string-array name="home_list_descriptions">
		<item>It is the old version of this awesome dashboard</item>
    </string-array>
    <string-array name="home_list_icons">
		<item>ic_na_launcher</item>
    </string-array>
    <string-array name="home_list_links">
		<item>https://github.com/jahirfiquitiva/Blueprint</item>
    </string-array>
</resources>
```