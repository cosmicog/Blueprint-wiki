Zooper widgets require a set of files that go into 4 folders: `bitmaps`, `fonts`, `iconsets`, `templates`

Those 4 folders are inside `src/main/assets`.

Copy your widgets files into the respective folders.

And that's it.

# Enabling the Zooper support in AndroidManifest.xml

Go to your project's AndroidManifest.xml, and search for the lines:
```xml
<!-- TODO: Remove comment marks to enable Zooper
<intent-filter>
	<action android:name="org.zooper.zw.TEMPLATES"/>
</intent-filter>
-->
```

```xml
<!-- TODO: Remove comment marks to enable Zooper
        <provider
                android:name=".zooper.TemplateProvider"
                android:authorities="${applicationId}.zwprovider"
                tools:ignore="ExportedContentProvider"/>
        -->
```

**Remove the comment marks to enable Zooper.**

# Modifying Zooper pack info.
Go to `res/values/kuper_configs.xml` and edit whatever you want.
I think the comments and names make the things self-explanatory, so it will be easy to do by yourself. [This page](https://github.com/jahirfiquitiva/Blueprint/wiki/Setting-up-kuper_configs.xml) explains it in full details though.

# Important for paid apps
Play encrypts paid apps, and that messes with the provider and Zooper.
So, to avoid problems with Zooper, additionally to your iconsets zips, unzip them and create a folder with its content, inside the iconsets folder too.
For example, if your iconset is named `WeatherIcons.zip`
- Copy it to: `assets/iconsets/`
- In `assets/iconsets/` create a folder with the name of your iconset zip, in this case `WeatherIcons`
- Extract the content of the iconset zip, in this case `WeatherIcons.zip` into `assets/iconsets/WeatherIcons` (or the folder you created in last step).
- Keep both the zip and the folder inside `assets/iconsets/`. The app will do the rest.
