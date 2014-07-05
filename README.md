TransparentSystemBar
====================    
###Transparent StatusBar and NavigationBar
```java
Window win = getWindow();
WindowManager.LayoutParams winParams = win.getAttributes();
winParams.flags |= WindowManager.LayoutParams.FLAG_TRANSLUCENT_STATUS;
winParams.flags |= WindowManager.LayoutParams.FLAG_TRANSLUCENT_NAVIGATION;
win.setAttributes(winParams);
```
or       
```xml
<style name="Translucent.SystemBar" parent="@android:style/Theme.Holo.Light">
    <item name="android:windowTranslucentStatus">true</item>
    <item name="android:windowTranslucentNavigation">true</item>
</style>
```		
---
###Transparent ActionBar(MEIZU SmartBar) ---------- style.xml    
```xml
<resources>
    <style name="AppBaseTheme" parent="android:style/Theme.DeviceDefault.Light">
    </style>

    <style name="AppTheme" parent="AppBaseTheme">
        <item name="android:actionBarStyle">@style/ActionBar</item>
    </style>

    <style name="ActionBar" parent="android:Widget.DeviceDefault.Light.ActionBar">
        <item name="android:background">@color/translucent_background</item>  (color = #000000)
        <item name="android:backgroundSplit">@color/translucent_background</item>
    </style>
</resources>
```
####MEIZU MX3 Screenshot
![MEIZU](https://github.com/gavinliu/TransparentSystemBar/raw/master/screen/S40705-164304.jpg)
####MOTO X Screenshot
![MOTO X](https://github.com/gavinliu/TransparentSystemBar/raw/master/screen/S40705-164305.png)
