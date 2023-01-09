# DEF CON: HDMI CEC 模糊

> 原文：<https://hackaday.com/2015/08/09/def-con-hdmi-cec-fuzzing/>

几乎所有足够先进的消费电子产品都采用了 HDMI。你可以在低端手机中找到它，没有 HDMI 的单板 Linux 计算机被认为是残废的。在 HDMI 规范中潜伏着一些有趣的东西，在 DEF CON 上，[ [Joshua Smith](https://twitter.com/kernelsmith) ]展示了 HDMI 的消费电子控制(CEC)部分，[并暴露了这一协议中的一些漏洞](https://www.defcon.org/html/defcon-23/dc-23-speakers.html#Smith)，这是所有具有 HDMI 端口的协议。

CEC 设计用于通过 HDMI 连接控制多个设备；它允许从机顶盒控制您的电视，从电视控制您的 DVD 播放器，并将文本从一个设备传递到另一个设备以在屏幕上显示。这是一条单线双向总线，带宽为 500 位/秒。有一些开源实现，如 [libCEC](http://libcec.pulse-eight.com/) 、 [Android HDMI-CEC](http://source.android.com/devices/tv/HDMI-CEC.html) ，甚至[一个 Arduino 实现](https://code.google.com/p/cec-arduino/)。微控制器与单个 CEC 引脚的接口电路非常简单，只需几个 jellybean 部件。

[Joshua]的作品基于[Andy Davis]在 black hat 2012[PDF]上的一次演讲，但在此基础上做了很大扩展。在查看了大量设备之后，[约书亚]能够在一台特定的松下电视和一台三星蓝光播放器中找到一些非常酷的漏洞。

某个针对松下电视的 CEC 命令发送了一个从 SD 卡上传新固件的命令。这有点奇怪，因为你会认为固件会自动从 SD 卡下载，就像成千上万的其他消费电子设备一样。对于三星蓝光播放器，发现 CEC 命令访问了一些 memcpy()调用，但它们还不容易被利用。

至于漏洞，[约书亚]有一些想法。游戏控制台和蓝光播放器无处不在，而圣杯——通过 HDMI 以太网通道(HEC)建立网络连接——是设备中城堡的钥匙*没有人*会想到仔细看看。

未来的工作包括重构当前代码，并深入研究更多设备。目前市场上有数百万个支持 CEC 的设备，而 CEC 命令本身并没有标准化。HDMI CEC 成为可靠工具的唯一方法是找出这些设备的命令。这是一项艰巨的工作，但却是一个伟大的行动号召，让更多的人研究这个非常有趣和通用的协议。