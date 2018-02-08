You will find the `AndroidManifest.xml` file under `app/src/main`. Here are the lines that you will need to edit:

## Package Name

```xml
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
          xmlns:tools="http://schemas.android.com/tools"
          package="jahirfiquitiva.apps.blueprint.demo">
````
In `AndroidManifest.xml`, find the lines shown above. In the last line of this block, replace `jahirfiquitiva.apps.blueprint.demo` with your app's package name. This is crucial for everything to function properly.

## Enabling donations
In `AndroidManifest.xml` you can find these lines:
```xml
<!-- Permission required for donations -->
<uses-permission android:name="com.android.vending.BILLING"/>
```
Be sure they are enabled if you plan on enabling donations to you. Otherwise, you are free to remove them.

Additionally, if you plan on enabling donations, you must also add a license key, even if you don't enable license check. That key works for both license check _and_ in-app purchases (donations). Learn how to do it [here](https://github.com/jahirfiquitiva/Blueprint/wiki/Setting-up-your-project----MainActivity.kt#what-does-every-line-do).