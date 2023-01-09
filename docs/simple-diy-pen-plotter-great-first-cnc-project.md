# 简单的 DIY 笔式绘图仪，伟大的第一个数控项目

> 原文：<https://hackaday.com/2015/01/16/simple-diy-pen-plotter-great-first-cnc-project/>

【Morten】最近忙着做一个[笔式绘图仪](http://hackaday.io/project/3840-laser-cutted-plotter)。这是一个简单而优雅的建筑，完全是他从头开始设计的。这里没有多余的琐碎部分。框架由激光切割的有机玻璃制成，如果你有激光切割机，这使得制作变得容易。两台 NEMA17 电机负责机器的移动。人们通过皮带前后移动笔托架。另一个通过激光切割齿轮连接到一个从喷墨打印机中取出的滚轴杆上，该滚轴杆在笔的下方向前和向后移动纸介质。

这里使用的软件链与我们在 Hackaday 上看到的其他廉价的 DIY CNC 机器相比有点不常见。[Morten]用 Rhino 创建他的几何图形，然后使用一个名为 Grasshopper 的插件来生成控制机器的 g 代码。g 代码通过 gRemote 发送到 Arduino，Arduino 通过[contraptor.org](http://www.contraptor.org/arduino-gcode-interpreter)g 代码解释器刷新。斜坡板接收 Arduino 产生的步进和方向信号，并相应地移动两个步进电机。

以典型的开放支持的方式，[Morten]让任何人都可以免费下载他的设计文件。他的绘图仪将笔从一边移动到另一边，将纸从前面移动到后面来绘制形状，但这不是绘图仪唯一的工作方式。看看这个[极坐标绘图仪](http://hackaday.com/2012/09/18/center-pivot-pen-plotter/)和这个[悬挂](http://hackaday.com/2013/05/17/android-pen-plotter-snaps-processes-and-prints-pictures/)的那个。

休息后请观看视频…

[https://www.youtube.com/embed/frAdpSLbBgo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/frAdpSLbBgo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)