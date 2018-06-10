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

#### v 1.2.0:
Easy as doing the same changes in the files that this [commit](https://github.com/jahirfiquitiva/Blueprint/commit/de649afc2a4c2bcadb502bab21ee2905848fd735) shows. :wink:

#### v 1.2.0:
Easy as doing the same changes in the files that this [commit](https://github.com/jahirfiquitiva/Blueprint/commit/fc306d4097433e4cfbad60de71776d4ef7787a04) shows. :wink:

#### v 1.1.8:
Easy as doing the same changes in the files that this [commit](https://github.com/jahirfiquitiva/Blueprint/commit/93f46d3596bde409752fd828af7f0a86b2099b46) shows. :wink:

#### v 1.1.5:
Easy as doing the same changes in the files that this [commit](https://github.com/jahirfiquitiva/Blueprint/commit/97ef8ba91458d5da9a9a2ea405440472f3da7242) shows. Basically just some minor version updates :wink:

#### v 1.1.4:
Easy as doing the same changes in the files that this [commit](https://github.com/jahirfiquitiva/Blueprint/commit/71343ab54e771df946a5e4d17ac4de44a8836b4b) shows. Basically just some minor version updates :wink:

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