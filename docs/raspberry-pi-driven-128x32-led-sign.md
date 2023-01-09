# 树莓 Pi 驱动 128×32 LED 标牌

> 原文：<https://hackaday.com/2013/11/14/raspberry-pi-driven-128x32-led-sign/>

看起来像商业 LED 显示标志…对吗？差远了。这是[Jon 的]一年前的一个项目，它是一个非常令人印象深刻的 [128×32 LED 显示板，使用单个 Raspberry Pi 驱动。](http://www.jonshouse.co.uk/ledsign.cgi)

它由八块“P10”32×16 的 LED 面板组成，这些面板是他从易贝买来的，安装在他自己建造的木框中。该显示器依靠单个 Raspberry Pi 运行，可以通过以太网端口接收来自任何设备的视频信号。各个电路板以一种相当奇怪的排列方式进行菊花链连接，以最大限度地减少电缆长度,[Jon]说这有助于快速记录数据——他能够解析每像素 2 位，以每秒 400 多帧的速度刷新显示器。

为了给显示器供电，他使用一个 ATX 电源，Pi 连接到备用 5V 电源线。这是为了避免可能导致 Pi 崩溃的电压降——当所有 led 都亮着时，显示器可以获得健康的 32A 电流。P10 使用移位寄存器串行加载像素数据。在任何时候，4096 像素显示器可以有 1024 个像素，这意味着需要一个相当快的时钟来更新显示。

[Jon]在他的博客上分享了所有的源代码，并对所有使用的系统进行了相当深入的解释。自己去看看吧，别忘了休息后留下来看看实际的展示！

[https://www.youtube.com/embed/zHSGtInrsDY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zHSGtInrsDY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)