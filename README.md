<p align="right"><a href="https://github.com/PicoSupport/PicoSupport/wiki/Unity-Call-Jar--and-Export-Jar" target="_blank">ExportJar</a></p>

# How to use the PackageManager

1. Open Unity, import picovrpackagemanager_v2.6.0.unitypackage, open AppList scene.

2. Create a new Unity project and copy the picovrpackagemanager_vxxx.jar in assets into the plugins-> Android directory of Unity project.

3. Modify the main activity: the android: name = "com. Picovr. Picopackagemanager. PicoVRPackageList"
 ![](https://github.com/PicoSupport/PackageManager/blob/master/assets/01.png)

4. Copy the script "PicoUnityActivity" under "Assets\Pvr_UnitySDK\Scenes\Examples" from Demo to any directory of Unity project.

5. Call Android interface method, string result = "";PicoUnityActivity. CallObjectMethod < string > (ref result, "getAllAppList");
Return value: result format
AppInfo [mPackageName= package name, mActivityName= application activity, mAppName= application name, mInstallTime= installation time, mSystemFlag= system application 0 not 1 yes]

Note: the Bundle Identifier of PlayerSetting in Unity should be consistent with the Android project.

# PackageManager使用方式

1.打开Unity，导入PicovrPackageManager_v2.6.0.unitypackage，打开AppList场景。

2.新建Unity工程，把assets中的中的picovrpackagemanager_vxxx.jar包，拷贝到Unity工程中Plugins->Android的目录下。

3.修改主activity：android:name="com.picovr.picopackagemanager.PicoVRPackageList"
![](https://github.com/PicoSupport/PackageManager/blob/master/assets/01.png)

4.将Demo中\Assets\Pvr_UnitySDK\Scenes\Examples路径下的PicoUnityActivity.cs脚本拷贝到Unity工程任意目录下。

5.调用Android接口方法，string result = "";PicoUnityActivity.CallObjectMethod <string>(ref result, "getAllAppList");

返回值：result格式

单个应用的基本信息：AppInfo [mPackageName=包名, mActivityName= 应用的activity, mAppName=应用名称, mInstallTime=安装时间, mSystemFlag=是否是系统应用 0不是 1是]

打包注意:Unity中PlayerSetting的Bundle Identifier要与Android工程保持一致。
