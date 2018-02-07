**This feature is completely optional. If you don't want to implement this, you can just ignore the content of this page.**

### Steps:
1. Create an account on [OneSignal](https://onesignal.com/).
2. Generate the required API keys following [this tutorial](https://documentation.onesignal.com/docs/generate-a-google-server-api-key).
3. Open this file: `app/build.gradle`
4. Just so you know, the comment marks are these: `/*` and `*/` and `//`
5. Do **NOT** sync gradle until you reach step 8. This is important.
6. Check these lines and remove the comments in them:
    - [#16](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/build.gradle#L16)
    - [#44](https://github.com/jahirfiquitiva/Blueprint/blob/sample/app/build.gradle#L44)
    - [#91](https://github.com/jahirfiquitiva/Blueprint/blob/master/app/build.gradle#L91)

    **Careful!** When you remove lines, the lines numbers will change, but you can easily find them by the comment marks.

7. Look for these keys and do as follows:
    - `onesignal_app_id` at line [#46](https://github.com/jahirfiquitiva/Frames/blob/sample/app/build.gradle#L46). Put the key OneSignal gives to you.
    - `onesignal_google_project_number` at line [#48](https://github.com/jahirfiquitiva/Frames/blob/sample/app/build.gradle#L48). Put the key Firebase gives to you.
8. *You can now sync gradle*

9. Go to this file: `app/src/main/kotlin/your/package/name/NotificationService.kt` and remove the comment marks at lines `18` and `27`.
10. Go to this file: `app/src/main/kotlin/your/package/name/MyApplication.kt` and remove the comment marks at lines `18`, `20`, `21`, `26`, `27` and `32`.

10. Clean and rebuild your project.

11. Run your app and test notifications from OneSignal's console.

12. If you want to change your notifications icon, just create a Vector Drawable XML icon and put it inside this folder: 
`app/src/main/res/drawable` with the name `ic_notifications.xml`. The name and folder are important and cannot be changed.