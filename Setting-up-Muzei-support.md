This is quite easy. Just open the `MuzeiService.kt` file under the `app/src/main/kotlin/your/package/name/`

You will find this simple line:
```kotlin
class MuzeiService:FramesArtSource("MyMuzeiService")
```

Just change the text inside the quotes from `"MyMuzeiService"` to the name you want to give it. Be sure it's unique to avoid conflicts.