<p align="right"><a href="https://github.com/PicoSupport/PicoSupport" target="_blank"> <img src="https://github.com/PicoSupport/PicoSupport/blob/master/Assets/home.png" width="20"/> </a></p>

# How to use the PackageManager

Note: Regarding java package creation and usege, please refer to [the Guideline](https://github.com/PicoSupport/PicoSupport/blob/master/Call%20And%20Export%20Jar.docx)

1. Open Unity, import picovrpackagemanager_v2.7.6.unitypackage, open AppList scene.

2. Create a new Unity project and copy the picovrpackagemanager_vxxx.jar in assets into the plugins-> Android directory of Unity project.

3. Modify the main activity: the android: name = "com. Picovr. Picopackagemanager. PicoVRPackageList"
 ![](https://github.com/PicoSupport/PackageManager/blob/master/assets/01.png)

4. Copy the script "PicoUnityActivity" under "Assets\Pvr_UnitySDK\Scenes\Examples" from Demo to any directory of Unity project.

5. Call Android interface method, string result = "";PicoUnityActivity. CallObjectMethod < string > (ref result, "getAllAppList");
Return value: result format
AppInfo [mPackageName= package name, mActivityName= application activity, mAppName= application name, mInstallTime= installation time, mSystemFlag= system application 0 not 1 yes]

Note: the Bundle Identifier of PlayerSetting in Unity should be consistent with the Android project.

