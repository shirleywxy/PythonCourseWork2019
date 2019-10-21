# PythonCourseWork2019
Python大作业交流展示
(注意Python的P要大写)

这里是一个Python大作业的交流展示分享的地方。

前期大家可以放自己的需求表在上面，虽然可能会有借鉴需求，同时也鼓励借鉴，但是互联网就是开放的，交流才会有进步，在学习的阶段更加鼓励能够把需求实现出来，这才是重要的。后面希望同学们在每个需求上增加相应项目的源代码链接，增加彼此交流。

## 目录

爬虫

* [我该去哪里](#whereCity)


目标检测

* [自动驾驶路况检测系统](#autoDrive)

个人博客

* [Hs bolg](http://hslovelal.top)

## 项目:我该去哪里(爬虫)
<span id="whereCity"/>

### Introduction

运用爬虫爬出国内各大城市的房价和薪资水平，对数据进行加工处理并展示到网站上，以较直观地方式展示各个城市的性价比。

### Features&Technology:

* 爬虫(对拉勾-BOSS直聘等招聘网站和链家-安居客等房产网站的分析和爬虫定制化制作)
* 网站搭建(Django作为后台，使用Vue+ElementUI等作为前端框架，MySql做数据库)

### Development

项目采用Git-flow作为Git工作流。采用敏捷开发模式。主要用PyCharm作为开发工具。

爬虫方面我们首先对各个网站做分析，找出可用数据的API接口，在本地调试好相应接口和数据返回，并将其存储到MySql数据库上，再将其放到腾讯云服务器上。后续可开放出API。
网站也架设在云服务器上。

后续可能会做Docker,CLI等。在功能点上，增加各个城市的男女比例，教育资源，医疗资源等来作为权重系数放在性价比评选中。用户可选中多个参数来得出自己的性价比。

### Thanks

如有雷同，纯属借鉴。



## 项目:自动驾驶路况检测系统
<span id="autoDrive"/>

### Introduction

输入照片，路况检测系统对其中的车辆和交通信号灯进行标注，如若发现信号灯则指示信号灯状态，并将结果进行实时反馈。

### Feature&Technology

将汽车前部安装的摄像头所拍摄到的照片作为输入，路况检测系统进行实时检测，识别出其中的车辆、交通信号灯。系统使用YOLOv2目标检测模型进行目标检测，并对检测到的车辆、交通信号灯使用方框进行标注。另外，检测系统使用Mobilenet图像分类模型判别路口交通信号灯的状态，是红灯还是绿灯。系统将检测结果进行实时反馈。

### Members

*    哈哈同学
*    丁同学  交互反馈：车辆目标检测结果标注，交通信号灯状态反馈
*    冯同学  目标检测：目标检测模型实现、训练、测试
*    黄同学  图像分类：图像分类模型实现、训练、测试
