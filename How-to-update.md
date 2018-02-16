## How to update?

Updating is pretty easy. You just need to upgrade Frames library version.

To do it, go to the `build.gradle` file inside `app` folder.

Then look for these lines:
```gradle
implementation('me.jahirfiquitiva:Blueprint:{latest version}@aar') {
    transitive = true
}
```

Replace `{latest version}` with the last version code from [![JitPack](https://jitpack.io/v/jahirfiquitiva/Blueprint.svg)](https://jitpack.io/#jahirfiquitiva/Blueprint)

Continue reading just in case bigger changes are required ;)


------

### Release Notes:
Whenever a new release is available **and** it requires extra changes for your setup, this is the section where they will be mentioned.

Check if you have done the required changes for the newest versions and do them if you haven't.

#### v 1.1.1:
1. Update your build.gradle to match the new [`app/build.gradle` file](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/build.gradle)
2. Update the proguard files:
    * [`proguard-android-optimize.txt`](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/proguard-android-optimize.txt)
    * [`proguard-rules.pro`](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/proguard-rules.pro)

#### v 1.0.4:

Update the [`proguard-rules.pro`](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/proguard-rules.pro) file.