## Optimal JSON format

```json
[
	{
		"name": "My wallpaper",
		"author": "Jahir Fiquitiva",
		"url": "https://www.mywebsite.com/wallpapers/my_wallpaper.png",
		"thumbnail": "https://www.mywebsite.com/wallpapers/thumbnails/my_wallpaper.png",
		"downloadable": true,
		"size": 345066,
		"dimensions": "1280 x 720 px",
		"copyright": "CreativeCommons Attribution-ShareALike"
	},
	{
		"name": "My other wallpaper",
		"author": "Jahir Fiquitiva",
		"url": "https://www.mywebsite.com/wallpapers/my_other_wallpaper.png",
		"thumbnail": "https://www.mywebsite.com/wallpapers/thumbnails/my_other_wallpaper.png",
		"downloadable": false,
		"copyright": "CreativeCommons Attribution-ShareALike"
	}
]
```

### Keywords explanation

| **Tag** | **Mandatory?** | **Description** | **Possible values** |
|:--------------:|:--------------:|:--------------------------------------------------------------------------------:|:------------------------------------------------------------------:|
| `name` | YES | Wallpaper name | Any text inside quotes `""` |
| `author` | NO | Wallpaper author | Any text inside quotes `""` |
| `url` | YES | The full-size/hi-res wallpaper url | Any url inside quotes `""` |
| `thumbnail` | NO | A downscaled/low-res/compressed version of your wallpaper | Any url inside quotes `""` |
| `downloadable` | NO | Whether users can download the wallpaper or not (True means yes. False means no) | `true` or `false` |
| `size` | NO | File size (**Warning:** size in **bytes** [1Mb=1024Kb, 1Kb=1024Bytes]) | Number like `1234` |
| `dimensions` | NO | Wallpaper dimensions with format `width x height px` | Any text inside quotes `""` |
| `copyright` | NO | It is always good to comply with licenses and copyright | Any text inside quotes `""` |


### Alternative keywords

Frames (Wallpaper library used in Blueprint) allows you to use other keywords for common tags:

|    **Tag**    |           **Possible keywords**               |
|:-------------:|:---------------------------------------------:|
| Thumbnail url | `thumbnail`, `thumbUrl`, `thumb`, `url-thumb` |
|   Dimensions  |           `dimensions`, `dimension`           |


### Migrating from another dashboard

Frames allows you to use the same format as your former dashboard. You just have to enable it in `app/src/main/res/values/frames_configs.xml` using the `use_old_json_format` bool. [More info here](https://github.com/jahirfiquitiva/Frames/wiki/Setting-up-frames_configs.xml)

### Finishing setup

When you have your JSON file ready. Upload it somewhere on the Internet and get its *raw* link. Then add it to [`strings.xml`](https://github.com/jahirfiquitiva/Frames/wiki/Setting-up-strings.xml)

And that's it! 😄 