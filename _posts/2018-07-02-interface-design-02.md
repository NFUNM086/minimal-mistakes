---
title:  "界面设计学习笔记-解决【_posts里文章不能在网页中显示】的问题"
modified: 2018-07-02 
categories: 
  - 界面设计
tags:
  - 笔记

sidebar:
  nav: "docs"
---
  
{% include base_path %}

{% include toc title="目录" %}


（第二篇界面设计学习笔记）

## 过程
- **发现问题**

网页中显示不出编辑了的文章（本应出现在“最新文章”下面）

![网页截图.png](https://upload-images.jianshu.io/upload_images/9400767-8e2e0000760e8e21.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- **查找原因**

明明利用[Hbuilder](https://baike.baidu.com/item/HBuilder/9145003?fr=aladdin)软件在_posts文件中编辑了如下图的markdown（以下简写md）文件

![_posts截图.png](https://upload-images.jianshu.io/upload_images/9400767-c1564659440193e4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

右边还有预览的视图

![Hbuilder截图.png](https://upload-images.jianshu.io/upload_images/9400767-4ab0c63d4a71467e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

登录gitee上也有commit的痕迹（如下图所示）

![commit截图.png](https://upload-images.jianshu.io/upload_images/9400767-549e28eaf104f051.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

项目里的“代码”里的_posts也有我编辑的几篇文章的存在

![gitee截图.png](https://upload-images.jianshu.io/upload_images/9400767-5b3cfa972d5f9ddd.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

包括在本地上的项目里也有我编辑的几篇文章存在

![本地文件截图.png](https://upload-images.jianshu.io/upload_images/9400767-9aaef0e019846e54.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- **寻求帮助**

寻求了同学和老师的帮助

![同学聊天记录截图.jpg](https://upload-images.jianshu.io/upload_images/9400767-49bc0fe4113ea1b4.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

尝试后

![github截图.jpg](https://upload-images.jianshu.io/upload_images/9400767-0355f1f6bb97be16.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

出现新的问题——转换到3.1.6分支后不能再转换到master分支

反思：3.1.6分支可以说只能是个草稿，而3.1.6和master分支里的东西互不影响

> *解决方法*
![github截图解决方法.png](https://upload-images.jianshu.io/upload_images/9400767-f1bad4139531e42c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
如上图所示，先按左下角的commit to 3.1.6的分支，然后再按右上角的push
原因是3.1.6分支里的东西没push完，只要push完了，就可以转换到master分支了



***
根据老师的指导
![修改前.png](https://upload-images.jianshu.io/upload_images/9400767-9e6109be060bc14b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

→

![修改后.png](https://upload-images.jianshu.io/upload_images/9400767-7cc7c079688debe0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

修改后，页面依旧有问题

增添了页头照片后

![出现原作者文章的页面.png](https://upload-images.jianshu.io/upload_images/9400767-139538c319c19066.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


竟然莫名其妙出现了原作者的文章，长达25页

- **反省和思考**
通过老师所说“重新fork，config可能全乱了”进行深入的思考。
猜测问题可能也只能出现在_config.yml
打开老师的_config.yml与我的进行**仔细对比**并修改，保证每一个空格、双引号、单引号等使用正确

![最终解决的截图.jpg](https://upload-images.jianshu.io/upload_images/9400767-6a3b689d11502db7.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

发现自己的代码和老师的代码存在很多不一样的小地方，但每一个细节都是致命的。
最终修改这个地方之后“文章不能正常显示”的错误被修正

## 总结
关于我的代码和别人（包括老师、同学）很多小地方不一样，我也不清楚原因，猜测是转换到3.1.6的分支，导致master分支混乱，直接导致_config.yml里面格式的错误，间接导致文章显示不出来的错误

*教训：yml格式很重要*
