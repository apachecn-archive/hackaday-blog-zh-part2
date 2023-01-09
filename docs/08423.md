# 树莓皮 GSM 帽子

> 原文：<https://hackaday.com/2015/02/28/raspberry-pi-gsm-hat/>

几天前发布了 Spark Electron，使任何拥有 Arduino IDE 的人都能够通过 GSM 网络发送数据。当然，电子只是一个连接到微控制器的 GSM 模块，[你可以用一个 Pi](http://hackaday.io/project/4462-raspberry-pi-fona-pihat) ，一些元件和一点导线做同样的事情。

构建相当简单——只有一个 Adafruit Fona、一个 2000 mah 的 LiPo 电池、一个充电控制器和一个花哨的 Hackaday Perma-Proto 帽子(T3 ),尽管一块 perf 板在 Perma-Proto 板的情况下也能很好地工作。连接就像电源、接地、TX 和 RX 一样简单。[有了几个库](https://learn.adafruit.com/fona-tethering-to-raspberry-pi-or-beaglebone-black)，你可以在任何有手机服务的地方通过互联网访问 Pi，或者在没有 WiFi 连接的情况下从 Pi 发送数据。

如果你决定复制这个项目，请注意你可以选择焊接 Fona 模块正面朝上或倒置。前者给你漂亮的闪烁的 led，而后者允许你访问 SIM 卡。确实是艰难的选择。