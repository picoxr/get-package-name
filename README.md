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
