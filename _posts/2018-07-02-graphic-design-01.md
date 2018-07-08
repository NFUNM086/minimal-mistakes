---
title:  "平面设计学习笔记-更换网站色调"
modified: 2018-07-02
categories: 
  - 平面设计
tags:
  - 笔记

sidebar:
  nav: "docs"
---
  
{% include base_path %}

{% include toc title="目录" %}

（第一篇平面设计学习笔记）

### 一、根据自己喜好设置网站的皮肤颜色
1. 在路径_sass-minimal-mistakes-skins里复制粘贴一个主题皮肤，然后自己重新命名。
这里我选择“_sunrise.scss”并重新命名为“_sunrisexu.scss”

![修改主题皮肤截图.png](https://upload-images.jianshu.io/upload_images/9400767-73a10afee524529f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

2.打开Hbuilder，根据自己喜好修改颜色
这里我改了这几处颜色

![自行修改颜色.png](https://upload-images.jianshu.io/upload_images/9400767-96c3ccf201b87330.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- 选色工具：[aTool在线工具的RGB颜色查询对照表](http://www.atool.org/colorpicker.php)
（可以自行调配颜色并实现RGB和十六进制自由转换）
- 颜色搭配工具：[Adobe Color CC](https://color.adobe.com/zh/create/color-wheel/base=2&rule=Analogous&selected=0&name=%E6%88%91%E7%9A%84%20Color%20%E4%B8%BB%E9%A1%8C&mode=rgb&rgbvalues=0.31890033788754785,0.7591057995239491,0.8235294117647058,0.32274452901997047,0.04550000000000004,0.91,1,0,0,0.91,0.5925608259668217,0.04550000000000004,0.7189087194526451,1,0.050000000000000044&swatchOrder=0,1,2,3,4 )
（可自动为你做出最好的颜色搭配选择）

### 二、色差的问题
当我修改好颜色，用手机打开想要检查时，发现了严重的色差问题

这是pc显示的颜色：

![pc显示颜色.png](https://upload-images.jianshu.io/upload_images/9400767-176577309a854fd6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

这是手机显示的颜色：

![手机显示颜色.jpg](https://upload-images.jianshu.io/upload_images/9400767-53f4d35554641fb5.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

相信我，这真的是同一个颜色，用电脑看和手机看色差真的很大：）
包括电脑截图发送到手机上看，也是有色差的
---
于是我进行了一系列的修改
最终根据先前设置好的页头照片确定主色调为蓝色
然后修改为如下图所示的色调

![最终确定的主题颜色页面.jpg](https://upload-images.jianshu.io/upload_images/9400767-1e42620fa49ddea0.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![修改页脚文字颜色前.jpg](https://upload-images.jianshu.io/upload_images/9400767-4d937ce3dc2b6b26.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

后面发现页脚文字的颜色和所在的背景的颜色太接近，难以辨认
于是又进行下一步的修改

![修改页脚文字颜色后.jpg](https://upload-images.jianshu.io/upload_images/9400767-0cb73ec056e5381f.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

然后也用手机打开网站（如下图所示）

![用手机打开网站截图1.jpg](https://upload-images.jianshu.io/upload_images/9400767-8cf8b861b56290eb.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![用手机打开网站截图2.jpg](https://upload-images.jianshu.io/upload_images/9400767-25e52ab94df444dc.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

最终完成了更换网站的颜色色调

### 三、反思
1. **网页设计配色原则**
a. 需要配色的是你的画布，而不是你的图片
b. 选择简单的灰色作为你网站的基调
c. 只选择一种颜色突出显示
d. 尽量不要使用颜色选择器右上角的颜色

![颜色选择器.png](https://upload-images.jianshu.io/upload_images/9400767-b9933c44c6ee32ff.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

2. **色差**指的是透镜成像的一个严重缺陷，色差简单来说就是颜色的差别，发生在以多[色光](https://baike.baidu.com/item/%E8%89%B2%E5%85%89)为光源的情况下，[单色光](https://baike.baidu.com/item/%E5%8D%95%E8%89%B2%E5%85%89/1168886)不产生色差。可见光的波长范围大约400至700纳米，不同波长的光，颜色各不相同，其通过透镜时的折射率也各不相同，这样物方一个点，在像方则可能形成一个色斑。色差一般有位置色差、放大率色差。位置色差使像在任何位置观察，都带有色斑或晕环，使像模糊不清，而放大率色差使像带有彩色边缘。[光学系统](https://baike.baidu.com/item/%E5%85%89%E5%AD%A6%E7%B3%BB%E7%BB%9F/5462197)最主要的功能就是消色差 。
3. **电脑和手机上显示的颜色色差较大的原因**
屏幕材质不一样，显示屏的[分辨率](https://baike.baidu.com/item/%E5%88%86%E8%BE%A8%E7%8E%87/213523?fr=aladdin)不一样手机和电脑屏幕的色域、色准不一样，如果你把两个都校准到同一色域（如sRGB）的话色彩会很相近。而显示屏的原因是因为与用的[液晶面板](https://www.baidu.com/s?wd=%E6%B6%B2%E6%99%B6%E9%9D%A2%E6%9D%BF&tn=SE_PcZhidaonwhc_ngpagmjz&rsv_dl=gh_pc_zhidao)，及出厂时的校准等有关，有的手机厂商为了讨好，把手机屏幕调得比较艳丽，传到电脑上就会出现色差较大的问题。



