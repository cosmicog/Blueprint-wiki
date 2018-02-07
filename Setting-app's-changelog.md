The changelog file can be found here: `res/values/changelog.xml`

Here's an example for you to understand how the new changelog structure works:
```xml
    <version title="v1.0.1"/>
    <item text="This is another version"/>
    <item text="Versions are shown in the order you put theme here"/>
    <item text="Bug fixes"/>
	
    <version title="v1.0.0"/>
    <item text="Initial Changelog"/>
    <item text="Bullet point here"/>
    <item text="More points"/>
    <item text=""/> <!-- this one is empty and therefore ignored -->
```

You can add as many versions as you want.