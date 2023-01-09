# 坦纳印刷电路板紫外线灯是如此明亮，你得戴上墨镜

> 原文：<https://hackaday.com/2014/03/06/face-tanner-pcb-uv-lamp-is-so-bright-you-gotta-wear-shades/>

当谈到用紫外线蚀刻印刷电路板时，太阳底下可能没有什么新东西，但是[Heliosoph]已经[对他买的一个二手制革工](http://heliosoph.mit-links.info/face-tanner-pcb-uv-lamp/)进行了更好的控制，现在可以在大约 50 秒内曝光他的电路板。

原始系统允许以 1 分钟为增量对 1-99 分钟的曝光时间进行编程。[Heliosoph]虽然照现在的样子它会很完美，但是灯是如此的强大，即使一分钟的曝光也太多了。当他打开东西时，他希望找到 TTL，并惊喜地发现了一个 [COP410L](http://pdf.datasheetcatalog.com/datasheet/nationalsemiconductor/DS006919.PDF) 微控制器和一个 MM5484 显示驱动器。遗憾的是，COP410L 的时钟范围太小，他不想超频。

[Heliosoph]基于 ATMega328P 构建了一个新的主板，带有一个回收的 16×2 LCD，他能够使用 Arduino IDE 附带的库轻松集成它。然后，他用一个固态继电器取代了 BT136 triac 灯开关，方便地将电子设备与主电源隔离。他使用 [M2tklib](http://code.google.com/p/m2tklib/) 重新设计了该设备的按钮，该设备支持过多的常用菜单功能。

如果你在整个 UV PCB 蚀刻过程中需要一些帮助，那么【CNLohr】的[这篇教程绝对不会错。](http://hackaday.com/2014/01/31/cnlohr-demos-his-photoetch-pcb-process/)