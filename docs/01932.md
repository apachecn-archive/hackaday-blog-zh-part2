# 4096 个 LED 意味着有史以来最大的 LED 立方体

> 原文：<https://hackaday.com/2012/10/21/4096-leds-means-the-biggest-led-cube-ever/>

犹他州的云计算管理和高性能计算公司 Adaptive Computing 需要一些非常酷的东西带到他们的贸易展览上。在混乱中创造秩序，并在数英里的线路中展示他们对细节的关注。他们决定建造最大的非商业 LED 立方体将是一个好项目，[，因此 16x16x16 All Spark 立方体诞生了](http://allsparkcube.com/wordpress/)。

All Spark Cube [由 10mm RGB led 和三英尺长的 16 ga 预镀锡铜线连接而成](http://allsparkcube.com/wordpress/?page_id=253)。[在这个视频](http://www.youtube.com/watch?feature=player_embedded&v=1bpgP0ck-c0)，【凯文】展示了构建单个行的过程；首先，将发光二极管放置在夹具中，将引线向下弯曲，并将总线焊接到每行 16 个独立的阳极上。

[构建硬件](http://allsparkcube.com/wordpress/?page_id=16)使用 16 个 Arduino Megas 和定制的屏蔽为 16×16 LED 网格供电。定制屏蔽为 led 提供 24V，为 Arduino 提供 5V，Arduino 板通过 RS485 连接相互通信，整个立方体通过 RS232 串行连接连接到计算机。

不可否认，这个软件还是有点花哨。致力于控制系统的适应性计算志愿者[斯潘塞]和[托马斯]在获得要显示的徽标和动画方面仍有一些问题。他们已经设法创建了一个控制应用程序来绘制单个像素，就像休息后看到的那样。

对于将近一英里的电线和一个夏天的工作来说还不错吧？

[https://www.youtube.com/embed/O-4EQPauUCI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/O-4EQPauUCI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)