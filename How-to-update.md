## How to update?

Updating is pretty easy. You just need to upgrade Frames library version.

To do it, go to the `build.gradle` file inside `app` folder.

Then look for these lines:
```gradle
implementation('com.jahirfiquitiva:Blueprint:{latest version}@aar') {
    transitive = true
}
```

Replace `{latest version}` with the last version code from [![JitPack](https://jitpack.io/v/com.jahirfiquitiva/Blueprint.svg)](https://jitpack.io/#com.jahirfiquitiva/Blueprint)

Continue reading just in case bigger changes are required ;)


------

### Release Notes:
Whenever a new release is available **and** it requires extra changes for your setup, this is the section where they will be mentioned.

Check if you have done the required changes for the newest versions and do them if you haven't.

#### v 1.4.9 and 1.5.0:
Check and apply the changes in [this commit](https://github.com/jahirfiquitiva/Blueprint/commit/4e3c7c9a74630b0a6ec4828e72725059019fd70c) and [this commit](https://github.com/jahirfiquitiva/Blueprint/commit/d710402720bcdff821309c0cb2e53fad5b7eef52)

#### v 1.4.2:
Check and apply the changes in [this commit](https://github.com/jahirfiquitiva/Blueprint/commit/799ea353b7bff49c48e8036613378d8cf71479c9)

#### v 1.4 and newer:
Check and apply the changes in [this commit](https://github.com/jahirfiquitiva/Blueprint/commit/2eaab89bc4b2400efec70caed600161d2a6b9c55).

Then delete the folder `.idea/libraries/` and all `build` folders, and then restart Android Studio using the `Invalidate Caches and Restart` option.

#### v 1.3.0:
Check the changes in [this commit](https://github.com/jahirfiquitiva/Blueprint/commit/96c8408e9ffa2fac283a35993cf56b9b948f8e3e)

#### v 1.2.9:
Provide links for your [`Privacy Policy` and/or `Terms and Conditions`](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/src/main/res/values/strings.xml#L31) in order to avoid issues with Play Store. [Generate them here](https://app-privacy-policy-generator.firebaseapp.com/).

#### v 1.2.8:
Update the [`app/build.gradle`](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/build.gradle), [`launchers.xml`](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/src/main/res/values/launchers.xml) and [`dependencies.gradle`](https://github.com/jahirfiquitiva/Blueprint/blob/sample/dependencies.gradle) files.

#### v 1.2.7:
Update your `AndroidManifest.xml` as done [in this commit](https://github.com/jahirfiquitiva/Blueprint/commit/d764658515e4454e361e766bdb33eeccf2b35798).

#### v 1.2.6:
Update the [`app/build.gradle`](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/build.gradle) and [`dependencies.gradle`](https://github.com/jahirfiquitiva/Blueprint/blob/sample/dependencies.gradle) files.

#### v 1.2.4:
Easy as doing the same changes in the files that this [commit](https://github.com/jahirfiquitiva/Blueprint/commit/2aec21edd02a797088172b2d694fe2ac517088bd) shows.

#### v 1.2.3:
Easy as doing the same changes in the files that this [commit](https://github.com/jahirfiquitiva/Blueprint/commit/de649afc2a4c2bcadb502bab21ee2905848fd735) shows.

#### v 1.2.0:
Easy as doing the same changes in the files that this [commit](https://github.com/jahirfiquitiva/Blueprint/commit/fc306d4097433e4cfbad60de71776d4ef7787a04) shows.

#### v 1.1.8:
Easy as doing the same changes in the files that this [commit](https://github.com/jahirfiquitiva/Blueprint/commit/93f46d3596bde409752fd828af7f0a86b2099b46) shows.

#### v 1.1.5:
Easy as doing the same changes in the files that this [commit](https://github.com/jahirfiquitiva/Blueprint/commit/97ef8ba91458d5da9a9a2ea405440472f3da7242) shows. Basically just some minor version updates :wink:

#### v 1.1.4:
Easy as doing the same changes in the files that this [commit](https://github.com/jahirfiquitiva/Blueprint/commit/71343ab54e771df946a5e4d17ac4de44a8836b4b) shows. Basically just some minor version updates.

#### v 1.1.3:
1. There's a new [`launchers.xml` file](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/src/main/res/values/launchers.xml) where you can remove the launchers you don't want to show in the "Apply" section.
2. There's a new [`bool` config](https://github.com/jahirfiquitiva/Blueprint/blob/121db2c562a7a9cd4dca1c812e4af4d203722be2/app/src/main/res/values/blueprint_configs.xml#L30) in [`blueprint_configs.xml`](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/src/main/res/values/blueprint_configs.xml) in case you want to hide the "General Information" in "Home" section.

#### v 1.1.1:
1. Update your build.gradle to match the new [`app/build.gradle` file](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/build.gradle)
2. Update the proguard files:
    * [`proguard-android-optimize.txt`](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/proguard-android-optimize.txt)
    * [`proguard-rules.pro`](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/proguard-rules.pro)

#### v 1.0.4:

Update the [`proguard-rules.pro`](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/proguard-rules.pro) file.