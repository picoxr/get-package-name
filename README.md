# PackageManager
Note: Regarding JAR file creation and usage, please refer to [the Guideline](https://github.com/picoxr/support/blob/master/How_to_use_JAR_file_in_Unity_project_on_Pico_device.docx)
## Introduction
This demo shows how to get installed package names on device.

## Class Name
android: name = "com. Picovr. Picopackagemanager. PicoVRPackageList"

## Interface
```
  String getAllAppList()
  ```
  return format:
  AppInfo [mPackageName= package name, mActivityName= application activity, mAppName= application name, mInstallTime= installation time, mSystemFlag= system application 0 not 1 yes]

