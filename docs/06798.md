# DIY 数据手套的柔性传感

> 原文：<https://hackaday.com/2014/08/11/flex-sensing-for-a-diy-data-glove/>

![cyber](img/94683e65205155bc463bcde1bf5c8167.png)

[Cyber]一直在测试虚拟现实体验的直观输入方法，这种方法比键盘或鼠标等古老设备更能让用户沉浸在虚拟世界中。到目前为止，他最大的兴趣之一是数据手套的想法，它可以与 Arduino Uno 交互，与 PC 接口。由于商业产品还没有现成的水平，[Cyber] [决定建造自己的](http://cybereality.com/?p=207)。

他从一个名为 [Pololu MinIMU-9 v2](http://www.pololu.com/product/1268) 的微型惯性测量单元开始，该单元可以跟踪三轴陀螺仪和加速度计的方向。USB 接口焊接到位，将电线连接到 Arduino Uno。在那里，他连接了一个来自 Spectra Symbol 的 flex 传感器(据称这是在[最初的任天堂电动手套](http://en.wikipedia.org/wiki/Power_Glove)中使用的),并通过跟踪他的一个手指的运动来演示该项目。随着手指弯曲，串行监视器上打印的输出发生了变化。

[赛博]仍然需要在这个系统上安装一个手套，并构建一个适当的位置跟踪方法，以便物理运动将反映在模拟中。

最近几个月，[赛博]的日常工作让他很忙，这迫使该项目暂时搁置。不过最近，[Cyber]已经成为一名活跃的成员，并对当地的[Orange County VR](http://orangecountyvr.com/)场景产生了影响，帮助建立了一种良好的开发文化，所以我们希望很快看到他的更多更新。

要查看他到目前为止做了什么，请单击页面顶部的链接，并在休息后查看视频:

[https://www.youtube.com/embed/CFBo-W8HB5k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CFBo-W8HB5k?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)