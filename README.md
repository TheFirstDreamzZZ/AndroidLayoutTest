# 安卓布局实验

## 实验1

###     实验要求：利用线性布局实现以下界面 

<img src="https://github.com/TheFirstDreamzZZ/AndroidLayoutTest/blob/master/app/ScreenShot/title1.png" width="500" />

[点此查看实验代码](https://github.com/TheFirstDreamzZZ/AndroidLayoutTest/blob/master/app/src/main/res/layout/test1.xml)</br>

其中，为了完成跟图上尽可能的相似，从网上copy了一段边框代码: </br>

```JAVA
<?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android">

    <stroke android:width="2dp" android:color="#666" />
</shape>
```

在res/drawable文件夹下创建xml文件，将代码粘贴进去</br>

引用在框架的background属性</br>

```JAVA
android:background="@drawable/buttonshape"
```

###     实验结果截图：

<img src="https://github.com/TheFirstDreamzZZ/AndroidLayoutTest/blob/master/app/ScreenShot/test1.png" width="500" />

## 实验二
