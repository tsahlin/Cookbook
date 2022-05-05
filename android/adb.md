# Android / adb command

- [Locations on Windows](#locations-on-windows)
- [Show help](#shop-help)
- [Show adb version](#shop-adb-version)
- [List available devices](#list-available-devices)
- [Start a shell for a device](#start-a-shell-for-a-device)
- [List users (profiles) on a device](#list-users-profiles-on-a-device)
- [Install an APK](#install-an-apk)

### Locations on Windows
```
C:\Program Files (x86)\Android\android-sdk\platform-tools
C:\Users\<user>\AppData\Local\Android\Sdk\platform-tools
```

### Show help
```
adb help
```

### Show adb version
```
adb version
```

### List available devices
```
adb devices
```

The first column in the list is the device **serial**, used with the `-s <serial>` flag in other commands. Can also be saved as an env variable:

```
set ANDROID_SERIAL=<serial>
```

### Start a shell for a device
```
adb shell
adb -s <serial> shell
```

### List users (profiles) on a device
```
adb shell pm list users
```

### Install an APK
```
adb install <file.apk>
```
