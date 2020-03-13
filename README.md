# 安卓布局实验

## 实验环境

* Windows10+Android Studio3.5.2

* AS采用安卓10

## 实验1

###     实验要求：利用线性布局实现以下界面 

<img src="https://github.com/TheFirstDreamzZZ/AndroidLayoutTest/blob/master/app/ScreenShot/title1.png" width="500" />

[点此查看实验代码](https://github.com/TheFirstDreamzZZ/AndroidLayoutTest/blob/master/app/src/main/res/layout/test1.xml)</br>

* 实验使用线性布局的嵌套来实现多行多列的效果

采用了button作为控件，为了完成跟图上尽可能的相似，从网上copy了一段边框代码: </br>

```JAVA
<?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android">

    <stroke android:width="2dp" android:color="#666" />
</shape>
```

在res/drawable文件夹下创建xml文件，将代码粘贴进去</br>

使用在button控件的background属性</br>

```JAVA
android:background="@drawable/buttonshape"
```

###     实验结果截图：

<img src="https://github.com/TheFirstDreamzZZ/AndroidLayoutTest/blob/master/app/ScreenShot/test1.png" width="375" />

## 实验二

###     实验要求：利用约束布局实现以下界面 

<img src="https://github.com/TheFirstDreamzZZ/AndroidLayoutTest/blob/master/app/ScreenShot/title2.png" width="500" />

[点此查看实验代码](https://github.com/TheFirstDreamzZZ/AndroidLayoutTest/blob/master/app/src/main/res/layout/test2.xml)</br>

本题参考了老师代码采用了TextView控件，以达到更好的相似度</br>

* 实验参考了官方文档的《使用 ConstraintLayout 构建自适应界面》
* 网址：[https://developer.android.google.cn/training/constraint-layout](https://developer.android.google.cn/training/constraint-layout)

利用可视化编程，给布局中的每个组件设置多个约束条件。</br>

主要用到以下几个功能：</br>

>> 1.用屏障功能实现不同控件的边的对齐</br>

>>> 绿色矩形右边和橙色矩形左边对齐，紫色矩形右边和橙色矩形右边对齐</br>

>> 2.给多个控件建立链的关系，使之在水平方向保持对齐</br>

>>> 绿、蓝、紫三个矩形对齐</br>

>> 3.利用Attributes窗口的Layout部分调整约束</br>

## 实验结果截图：</br>

<img src="https://github.com/TheFirstDreamzZZ/AndroidLayoutTest/blob/master/app/ScreenShot/test2.png" width="375" />

## 实验三

###     实验要求：利用表格布局实现以下界面

<img src="https://github.com/TheFirstDreamzZZ/AndroidLayoutTest/blob/master/app/ScreenShot/title3.png" width="500" />

[点此查看实验代码](https://github.com/TheFirstDreamzZZ/AndroidLayoutTest/blob/master/app/src/main/res/layout/test3.xml)</br>

表格布局中，用TableRow设置行，行数由TableRow决定，多行则需要多个TableRow，而列数为控件最多的那行的控件数决定。</br>

课件上有类似的题目，主要采用布局的列拉伸的方法实现：</br>

```JAVA
android:stretchColumns="1"
```

将文字放在拉伸的列中，就能使得其他控件占用最小空间。</br>

利用gravity属性让文字居右显示(默认为居左)</br>

其中，分割线我是参考了百度上别人的博客：</br>

* 网址为:[https://blog.csdn.net/liaoxueli/article/details/84183690](https://blog.csdn.net/liaoxueli/article/details/84183690)</br>

代码实现如下：</br>
```JAVA
<View
        android:layout_height="1dp"
        android:background="#B7B7B7" />
```

其中要保持所有控件的内边距(padding)属性一致，才能使得界面更加整齐。</br>

## 实验结果截图:</br>

<img src="https://github.com/TheFirstDreamzZZ/AndroidLayoutTest/blob/master/app/ScreenShot/test3.png" width="375" />

## 实验总结：</br>

>> 本次实验让我更加深刻的了解各种布局的用法，熟悉了多个控件的属性的用法，在不断地琢磨和搜索解决方案中，更加能理解布局的结构。学习了很多知识，比如使用线性布局来创建多行多列的效果，使用可视化调整控件，学习分割线等...。这次实验是迈进Android开发的第一步，相信在以后的学习中，我能更加顺利。
