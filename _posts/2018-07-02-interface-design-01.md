---
title:  "界面设计学习笔记之解决【部署失败】和【网页不能正常显示】的问题"
modified: 2018-07-05 
categories: 
  - 界面设计
tags:
  - 学习笔记
---

{% include base_path %}

{% include toc title="目录" %}


（第一篇界面设计学习笔记）

# **部署失败**
- **问题出现**

![部署失败的截图.jpg](https://upload-images.jianshu.io/upload_images/9400767-79e6ad7bc478c6cc.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- **尝试解决**

根据错误信息的提供，找到_data/navigation.yml中的第5行，发现-前多了一个空格，没有与其他行对齐
于是进行了修正（如下图所示）

![yml格式修正后.png](https://upload-images.jianshu.io/upload_images/9400767-bf9a7001997428f8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

Gitee Pages服务能正常操作，有网站地址出现（如下图所示）

![pages服务截图.png](https://upload-images.jianshu.io/upload_images/9400767-689cc4e3e85ab47a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---

# **网页不能正常显示**
- **问题出现**

![网页不能正常显示.jpg](https://upload-images.jianshu.io/upload_images/9400767-0cc367f4f0e88063.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- **寻找错误**

猜想产生错误的地方（因为当时只改了这里）

![修改个人信息.jpg](https://upload-images.jianshu.io/upload_images/9400767-c18179a201ba6801.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

仔细与同学、老师的代码尽心对照，没找到错误


> **最后的解决方法**
——点击“强制同步”的按钮
![强制同步.png](https://upload-images.jianshu.io/upload_images/9400767-cfbe5275c8b56c09.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![强制同步确认页面.png](https://upload-images.jianshu.io/upload_images/9400767-709f9143873f5a7a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


 ---
- **反思**
在Hbuilder上编写的代码只是push到Github仓库，并没有与Gitee线上同步，所以必须【强制同步】，网站才有应该有的变化