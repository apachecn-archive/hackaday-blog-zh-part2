# 制造者集会上的蓝牙设备

> 原文：<https://hackaday.com/2014/09/23/bluetooth-thingies-at-maker-faire/>

[https://www.youtube.com/embed/fhfju-ON1R8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fhfju-ON1R8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

如果您没有注意到，新开发板的一个更受欢迎的主题是蓝牙。将蓝牙 4.0 模块放在电路板上，你就真的有东西了:几乎每部手机都有它，低能耗标签非常适合电池供电的物联网。

这些板中的大多数都有一点不足。将蓝牙模块放在电路板上是一回事，但构建与电路板交互的软件完全是另一回事。揭示小时创作[是与他们的 Tah 板](http://tah.io/)的趋势相反。基本上，它是带有 btle 模块的标准 Arduino 兼容板。他们所做的是为 iOS 和 Android 添加软件，使构建东西变得容易。

[https://www.youtube.com/embed/OmIB-ttazag?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/OmIB-ttazag?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

把蓝牙放在单板上是一回事，但是把蓝牙放在 *everything* 上怎么样？ [SAM Labs 在 Maker Faire 上展示了他们的物联网](http://samlabs.me/)，包括 led、按钮、风扇、马达、传感器，以及几乎所有你能想象到的电子元件。

所有这些小电路板都配有蓝牙模块和电池。该系统的软件是一个图形界面，允许你在所有东西之间画虚拟线。将一个按钮连接到软件中的一个 LED 上，当按钮被按下时，LED 就会亮起。在电脑上移动你的鼠标，按下这个按钮就会启动一个马达。

有几个 API 也打包到编程环境中——在展台上，你可以打开一个冰箱(装满了不花 5 美元的冷饮，这是对 faire 的一个惊喜),它会发布一条推文。