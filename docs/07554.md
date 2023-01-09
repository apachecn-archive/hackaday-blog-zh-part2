# 树莓派的 2 美元调频发射机

> 原文：<https://hackaday.com/2014/11/12/2-fm-transmitter-for-rasberry-pi/>

我们喜欢改变用途的消费设备。[托拜厄斯]给我们发来了他的项目链接，该项目使用一种廉价的停产手机配件来制造一种由树莓皮控制的调频无线电发射机。

索尼-爱立信 MMR-70 无线电发射机显然是用来连接手机和播放音乐的。但是有问题的随身听手机有点旧了，所以你可以在转售市场上买到便宜的发射机。使发射机更有趣的是，你可以激活和关闭收音机，改变频率或输出功率，甚至发送无线电数据系统电台和歌曲信息。

[原来](http://www.mikrocontroller.net/topic/252124)(德语链接)这些收音机有一个 AVR ATMega32 微控制器和一个 NS73 无线电发射模块，可以完全通过 I2C 控制。([示意图此处为 PDF](http://www.mikrocontroller.net/attachment/140251/MMR70.pdf) 。)这些单元还在周围散布着方便的[测试点。一旦确定了测试点，就可以完全忽略板载 AVR 微控制器，直接使用 Raspberry Pi 的 I2C 输出来控制 FM 发射器模块。](https://github.com/Manawyrm/FMBerry/blob/master/HARDWARE.md)

这就是[托拜厄斯]介入的地方。他为 Raspberry Pi 编写了一个 I2C 守护程序，可以让你通过简单的命令控制调频发射机。你所要做的就是焊接一堆测试点，安装[Tobias]的软件，写一个批处理脚本，然后你就可以上电视了。例如，这使得为在线流式音频制作一个 FM 无线电转播器成为一个一天的项目。你可以在 youtube 上看到他的[工作实例。当然，你会想要一个](https://www.youtube.com/watch?v=NJRADd7C6rs)[基于网络的远程控制界面](https://github.com/akkinitsch/FMBerryRemote)与之搭配。

如果你对黑客感兴趣，并且没有树莓 Pi 应用程序的想法，那么 [Sparkfun 曾经出售 NS73 无线电发射机](https://www.sparkfun.com/products/retired/8452)，所以你可以找到许多关于芯片的好信息。我们很想看到一个独立的广播小发明，它实际上利用了板载 AVR 芯片，但我们对[Tobias]让 Raspberry Pi 版本变得如此容易理解表示敬意。