You can easily modify both the launcher icons and system (function) icons in Blueprint.

## Modifying launcher icons
To modify the launcher icons which are displayed in the Apply section, add your own replacements to `app/src/main/res/drawable-nodpi`. Choose any launcher icon you'd like to modify from [here](https://github.com/jahirfiquitiva/Blueprint/tree/master/library/src/main/res/drawable-nodpi) (launcher icon assets begin with `ic_`, and create a replacement file (PNG, 512x512 pixels). Drop it into the previously mentioned path, and you're done.

## Modifying system (function) icons
Replacing the system icons is very similar to modifying the launcher ones. Navigate to `app/src/main/res` and create a folder called `drawable` there. Choose any system icon you'd like to modify from [here](https://github.com/jahirfiquitiva/Blueprint/tree/master/library/src/main/res/drawable) (system icon assets begin with `ic_`), and create a replacement file (SVG, 24x24 pixels). Go to [this website](http://inloop.github.io/svg2android/) and convert your SVG into an XML vector drawable. Drop the generated file into the previously mentioned path, and you're done.