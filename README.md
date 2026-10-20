<div align="center">

  <h1>Orbit Mobile</h1>

  <p>
    A free, open-source media app for your phone, your desktop, and the TV you already own.
    <br />
    Bring your own sources. Orbit turns them into a library with artwork, ratings, subtitles, and your place saved on every screen.
  </p>

  [GitHub releases](https://github.com/shubh152205/OrbitMobile/releases/latest)

</div>

## Get Orbit Mobile

- [Android APK](https://github.com/shubh152205/OrbitMobile/releases/latest)

## Build from source

```bash
git clone https://github.com/shubh152205/OrbitMobile.git
cd OrbitMobile
```

### Android

Android development requires Android Studio and the Android SDK.

```bash
./gradlew :androidApp:assembleFullDebug
```

### iOS

iOS development requires macOS and Xcode.

```bash
env NUVIO_IOS_DISTRIBUTION=full xcodebuild \
  -project iosApp/iosApp.xcodeproj \
  -scheme iosApp \
  -configuration Debug \
  -sdk iphonesimulator \
  -derivedDataPath build/ios-derived-full-simulator \
  CODE_SIGNING_ALLOWED=NO \
  build
```

The shared app is built with Kotlin Multiplatform and Compose Multiplatform.

## License

[GNU General Public License v3.0](./LICENSE)
