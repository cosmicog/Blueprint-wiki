Kustom require a set of files that go into 4 folders, depending on the asset: `komponents`, `wallpapers`, `widgets`, `lockscreens`.

Those 4 folders are inside `src/main/assets`.

Copy your widgets files into the respective folders, keeping these things in mind:

- `komponents`: the file must end with `.komp.zip` extension.
- `wallpapers`: the file must end with `.klwp.zip` extension.
- `widgets`: the file must end with `.kwgt.zip` extension.
- `lockscreens`: the file must end with `.klck.zip` extension.

Check the sample app assets for a real example.

And that's it.

# Enabling the Kustom support in AndroidManifest.xml

Go to your project's AndroidManifest.xml, and search for the lines:

```xml

	<!-- TODO: Remove comment marks to enable Kustom Skins
        * Remove intent-filter action lines according to your needs.
		* If you're not going to provide one of the options, remove its respective line.
        <provider
                android:name="org.kustom.api.Provider"
                android:authorities="${applicationId}.kustom.provider"
                android:exported="true"
                tools:ignore="ExportedContentProvider">
            <intent-filter>
                <action android:name="org.kustom.provider.WALLPAPERS"/>
                <action android:name="org.kustom.provider.WIDGETS"/>
                <action android:name="org.kustom.provider.KOMPONENTS"/>
                <action android:name="org.kustom.provider.LOCKSCREENS"/>
            </intent-filter>
        </provider>
        -->
```

**Remove the comment marks to enable Kustom.**

**Also, remove the intent filters for the things you won't use or include.**


# Modifying Kustom pack info.
Go to `res/values/kuper_configs.xml` and edit whatever you want.
I think the comments and names make the things self-explanatory, so it will be easy to do by yourself. [This page](https://github.com/jahirfiquitiva/Blueprint/wiki/Setting-up-kuper_configs.xml) explains it in full details though.