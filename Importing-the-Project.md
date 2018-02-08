### For Android Studio older than 3.0, install the Kotlin plugin for Android Studio
1. Go to File🡒Settings🡒Plugins🡒Install plugin.
2. Search for Kotlin plugin & install it.
4. Restart Android Studio when install finished.

## Importing the project to Android Studio
- Download the project from Github Page by using `clone`, the download button located under `code` tab, or just click [this link](https://github.com/jahirfiquitiva/Blueprint/archive/sample.zip)
- Unzip the master project and put into your desired directory.
- Open Android Studio and open the downloaded project using 'Open an existing Android Studio project' option.

## Changing the app's package.
- Expand following directory `/app/src/kotlin`.
- Right click on `kotlin` directory.
- Choose `New 🡒 Package`.
- Enter your package name into the window eg. `com.package.name`.
- From expanded default package directory `jahirfiquitiva/apps/blueprint/demo/` select all `*.kt` files and cut them (using ctrl+x).
- Paste these files into your own package directory.
- Delete default (now empty) package directory.