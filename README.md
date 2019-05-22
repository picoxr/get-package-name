# PackageManager

JAR file, demo apk are in /resource.    
Note: Regarding JAR file creation and usage, please refer to [the Guideline](https://github.com/picoxr/support/blob/master/How%20to%20Use%20JAR%20file%20in%20Unity%20project%20on%20Pico%20device.docx)

## Introduction
This demo shows how to get installed package names on device.

## Class Name
```
com.picovr.getpackage.GetPackageClass
```

## Interface
```
String getAppString(Context context)    
```
  return format:
  AppInfo [mPackageName= package name, mActivityName= application activity, mAppName= application name, mInstallTime= installation time, mSystemFlag= system application 0 not 1 yes]&

## Sample Code
```
AndroidJavaObject ajo = new AndroidJavaObject("com.picovr.getpackage.GetPackageClass");
AndroidJavaObject context = new AndroidJavaClass("com.unity3d.player.UnityPlayer").GetStatic<AndroidJavaObject>("currentActivity");

string apps = ajo.Call<string>("getAppString", context);
```
