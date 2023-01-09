# 一个简单的跑步者 GPS 记录器

> 原文：<https://hackaday.com/2014/11/23/a-simple-runners-gps-logger/>

[丹尼尔]获得了明尼苏达大学儿童早教展望基金的资助，因此负责创造一些东西。 [他建造了一个跑步者的 GPS 记录器](https://sites.google.com/a/umn.edu/tayl0518-runners-gps/)，配有一个屏幕，可以显示跑步者当前行进的距离、行进该距离所用的时间，除此之外别无其他。没有开始/停止，没有暂停，什么都没有。可以把它想象成一个精简的 GPS 记录器，一个最小可行产品的完美例子，以及一个用 ARM micro 把地图放到屏幕上的很好的介绍。

该构建包括 LPC1178 ARM Cortex M3 微控制器、显示器、GPS 单元和电池，没有太多其他东西被塞进数控铣削的外壳中。地图来自 [OpenStreetMap](http://www.openstreetmap.org/) ，存储在 microSD 卡上。[的大部分文件在 GitHub](https://github.com/dbtayl/Runner-s-GPS) 上都有，案例设计的文件很快就会上传。

用来制造外壳的数控机器(丹尼尔)本身就是一件艺术品。[我们去年推出了这款产品](http://hackaday.com/2013/08/16/101459/)，它足以处理 10 密耳走线的 PCB。出色的工作，虽然有这种能力，我们想知道为什么跑步者的 GPS PCB 是奥什公园紫色。