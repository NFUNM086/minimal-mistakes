---
title:  "界面设计学习笔记-解决【Github链接404】的问题"
modified: 2018-07-02 
categories: 
  - 界面设计
tags:
  - 笔记
---

{% include base_path %}

{% include toc title="目录" %}


（第三篇界面设计学习笔记）

### 问题出现

点击左下角的GitHub链接

![Github链接.png](https://upload-images.jianshu.io/upload_images/9400767-c982a3ef9ccc319a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

网页打不开，显示404

![github链接404.jpg](https://upload-images.jianshu.io/upload_images/9400767-75997a820e0fda4b.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 检查修正
检查代码中的url
进行第一次尝试修正

![检查url第一次.png](https://upload-images.jianshu.io/upload_images/9400767-1b2c02b2d89b7e44.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

仍然404
再次观察发现链接url有问题（如下图所示）

![发现url有问题.png](https://upload-images.jianshu.io/upload_images/9400767-a094459dae976483.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

进行第二次尝试修改

![检查url第二次.png](https://upload-images.jianshu.io/upload_images/9400767-5b77340bc51bcb2f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

Github链接正常显示

![Github链接正常打开.png](https://upload-images.jianshu.io/upload_images/9400767-6f34d69f4834af9b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 总结
url格式很重要，链接不能正常打开/404原因大部分出现在url上
