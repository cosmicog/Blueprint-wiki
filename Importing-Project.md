## Importing the project to Android Studio

**First of all install Android Studio Kotlin plugin**
1. Go to File🡒Settings🡒Plugins🡒Install plugin
2. Search for Kotlin plugin
3. Install it
4. Restart Android Studio when install finished

**How to import Blueprint project into Android Studio**
- Download the project from Github Page by using `clone or download` button located under `code` tab. Or just click [this link](https://github.com/jahirfiquitiva/Blueprint/archive/sample.zip)
- Unzip the master project and put into desired directory.
- Open Android Studio and open previously downloaded project using 'Open an existing Android Studio project' option.

## Changing the app's package.

- Expand following directories `/app/src/kotlin`.
- Right click on `kotlin` directory.
- Choose `New 🡒 Package`.
- Enter your package name into the window eg. `com.package.name`.
- From expanded default package directory `jahirfiquitiva/apps/blueprint/demo/` select all `*.kt` files and cut them (using ctrl+x).
- Paste these files into your own package directory.
- Delete default (now empty) package directory.