# Adding a single icon example
There are 2 things you need to get first;
1. Of course the drawable icon file,
2. The **main activity's class name** of your package. For this example, we're going to use Google's Messaging app. And maybe the most time eater process about creating an icon pack is finding each package's main activity name. For our example app, it's:`com.google.android.apps.messaging.ui.ConversationListActivity`

Copy your big, perfectly sized (I recommend 288x288) icon to the `drawable-nodpi` folder, let's say, named `com_google_android_apps_messaging.png` and do the **6 steps below** for your icon.

---
** 1. Inside the  `app/src/main/res/xml/appfilter.xml` file **

by using `pkg_name/activity_class_name` and `png_name`, create the item below:

```
    <item
        component="ComponentInfo{com.google.android.apps.messaging/com.google.android.apps.messaging.ui.ConversationListActivity}"
        drawable="com_google_android_apps_messaging" />
```

** 2. Inside the `app/src/main/res/xml/appmap.xml` file **

`activity_class_name` + `png_name`

```
    <item
        class="com.google.android.apps.messaging.ui.ConversationListActivity"
        name="com_google_android_apps_messaging" />
```

** 3. Inside the  `app/src/main/res/xml/drawable.xml` file **

under title All(or your choice) `png_name`

```
    <item drawable="com_google_android_apps_messaging" />
```

** 5. Inside the  `app/src/main/res/xml/theme_resources.xml` file**

pkg_name/activity_class_name + png_name

```
    <AppIcon
        name="ComponentInfo{com.google.android.apps.messaging/com.google.android.apps.messaging.ui.ConversationListActivity"
        image="com_google_android_apps_messaging" />
```

** 6. Inside the  `app/src/main/res/values/icon_pack.xml` file **

under all and icon_pack arrays (and your arrays); `png_name`

```
        <item>com_google_android_apps_messaging</item>
```

---
Finally, you can copy, needs-to-be-copied files described in previous tutorial to the assets directory, here's how I do in a terminal inside the project folder(`my_icon_pack` or `Blueprint`)
```bash
username@unixpc:~/android_projects/my_icon_pack$ cp app/src/main/res/xml/appfilter.xml app/src/main/res/xml/drawable.xml app/src/main/res/xml/themecfg.xml app/src/main/res/xml/themeinfo.xml app/src/main/assets/
```
