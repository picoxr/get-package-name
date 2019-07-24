# PackageManager

JAR file, demo apk are in /resource.    
Note: Regarding JAR file creation and usage, please refer to [the Guideline](http://static.appstore.picovr.com/docs/JarUnity/index.html)

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
