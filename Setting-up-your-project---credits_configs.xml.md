Open `credits_configs.xml` file that is located in `/app/src/main/res/values/credits_configs.xml`

This file allows you to modify cards in the about screen and it looks like this:
````xml
<resources xmlns:tools="http://schemas.android.com/tools" tools:ignore="MissingTranslation">

    <string-array name="credits_photos" formatted="false" tools:ignore="TypographyDashes">
        <item>https://lh3.googleusercontent.com/-0mdcClKXlgM/AAAAAAAAAAI/AAAAAAAAAAA/xgdLWeAg7pM/s120-c/photo.jpg</item>
        <item>https://ssl.gstatic.com/images/branding/product/2x/avatar_square_grey_512dp.png</item>
    </string-array>

    <string-array name="credits_titles">
        <item>Your Name</item>
        <item>Another Name</item>
    </string-array>

    <string-array name="credits_descriptions">
        <item>Details of first credited person</item>
        <item>Details of another credited person</item>
    </string-array>

    <string-array name="credits_buttons">
        <item>Google+|Instagram</item>
        <item>Facebook|Website|Twitter</item>
    </string-array>

    <string-array name="credits_links">
        <item>https://www.google.com/+JahirFiquitivaR|http://instagram.com/jahirfiquitiva</item>
        <item>https://facebook.com/|https://www.jahirfiquitiva.me/|https://twitter.com/jahirfiquitiva</item>
    </string-array>
</resources>
````
It works in a very simple way. By default each `string-array` has 2 `<item>` tags. This makes the about section display 2 cards with app creators.

If you want to add/remove a number of cards in about screen, simply add/remove `<item>` tags.

## What does each `string-array` do

**In order to add your text or link, simply paste it between `<item></item>` tags**

- `<string-array name="credits_photos" formatted="false" tools:ignore="TypographyDashes">`
This `string-array` holds links to avatars/profile pictures that will be displayed in card(s).
**Keep in mind, that it must be a RAW link, that leads to the plain image file and not a sharing page, like you normally get by sharing files from most popular cloud services**. You can find tutorials on how to get RAW links from cloud services like *Dropbox* or *Google Drive* in the internet.

- `<string-array name="credits_titles">`
This `string-array` holds creators' names

- `<string-array name="credits_descriptions">`
This `string-array` holds creators' descriptions

- `<string-array name="credits_buttons">`
This `string-array` holds buttons that will have links to your webpages. You can add multiple buttons here by sepparating them with `|` sign eg. `Link name1|Link name2`. Following this example, the card in about screen will display 2 buttons labeled `Link name1` and `Link name2` that will open webpages that you will set up in an `string-array` below.

- `<string-array name="credits_links">`
This `string-array` holds links that will *hide* under buttons you've set up above. It works in the same way as credit buttons. **Make sure to add the same number of links and buttons separated by `|` sign.**