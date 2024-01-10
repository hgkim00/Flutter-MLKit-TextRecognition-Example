# datascience_camp_2024_practice

### Version Info

```bash
Flutter 3.10.5 • channel stable • https://github.com/flutter/flutter.git
Framework • revision 796c8ef792 (7달 전) • 2023-06-13 15:51:02 -0700
Engine • revision 45f6e00911
Tools • Dart 3.0.5 • DevTools 2.23.1
```

### Package Version Info

```yaml
dependencies:
  flutter:
    sdk: flutter

  cupertino_icons: ^1.0.2

  google_mlkit_text_recognition: ^0.8.1
  camera: ^0.10.5+2
  permission_handler: ^10.3.0
```

### mlkit 관련 android 설정

- android > app > build.gradle

```gradle
android {
    ...

    compileSdkVersion 33    // 수정

    defaultConfig {
        ...
        minSdkVersion 22    // 수정
        targetSdkVersion 32 // 수정
        ...
    }

    ...
}
```

- android > app > src > main > AndroidManifest.xml

```xml
<manifest xmlns:android="http://schemas.android.com/apk/res/android">
    <!-- 추가 -->
    <uses-permission android:name="android.permission.CAMERA"/>

    ...

</manifest>

```
