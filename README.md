# PackageManager
Note: Regarding JAR file creation and usage, please refer to [the Guideline](https://github.com/picoxr/support/blob/master/How%20to%20use%20JAR%20file%20in%20Unity%20project%20on%20Pico%20Device.docx)
## Introduction
This demo shows how to get installed package names on device.

## Class Name
```
android: name = "com. Picovr. Picopackagemanager. PicoVRPackageList"
```

## Interface
```
  String getAllAppList()
  ```
  return format:
  AppInfo [mPackageName= package name, mActivityName= application activity, mAppName= application name, mInstallTime= installation time, mSystemFlag= system application 0 not 1 yes]

