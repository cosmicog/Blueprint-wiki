Open build.gradle file that is located in `app/build.gradle`.

All we care about is `applicationId` which is inside this group:
````kotlin

    defaultConfig {
        applicationId  'jahirfiquitiva.apps.blueprint.demo'
        minSdkVersion project.ext.minSdk
        targetSdkVersion project.ext.targetSdk
        versionCode project.ext.versionCode
        versionName project.ext.versionName
        vectorDrawables.useSupportLibrary = true
    }

````

You need to change `applicationId` in this file in order to change your app's package name. To do this, simply change `'jahirfiquitiva.apps.blueprint.demo'` to your own package name eg. `'your.package.name'`