# How to use PackageManager

Note: Regarding JAR file creation and usage, please refer to [the Guideline](https://github.com/PicoSupport/PicoSupport/blob/master/How_to_use_JAR_file_in_Unity_project_on_Pico_device.docx)

1. Modify the main activity: the android: name = "com. Picovr. Picopackagemanager. PicoVRPackageList"
 ![](https://github.com/PicoSupport/PackageManager/blob/master/assets/01.png)

2. Interface 
String getAllAppList()
Return value: string
AppInfo [mPackageName= package name, mActivityName= application activity, mAppName= application name, mInstallTime= installation time, mSystemFlag= system application 0 not 1 yes]

Note: the Bundle Identifier of PlayerSetting in Unity should be consistent with the Android project.

