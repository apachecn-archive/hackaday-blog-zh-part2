# 使用 RTL-SDR 测量滤波器和 VSWR

> 原文：<https://hackaday.com/2015/03/14/measuring-filters-and-vswr-with-rtl-sdr/>

无处不在的 USB 电视调谐器加密狗再次证明了自己不仅仅能够接收广播电视。在 RTL-SDR 博客上，有一篇关于使用廉价易贝噪声源和 RTL-SDR 加密狗测量滤波器特性[的教程。](http://www.rtl-sdr.com/rtl-sdr-tutorial-measuring-filter-characteristics-and-antenna-vswr-with-an-rtl-sdr-and-noise-source/)

对于本教程，设备的关键部分是一个 BG7TBL 噪声源，从通常的在线零售商那里获得。只需几个连接器，就可以在该噪声源和 RTL-SDR 加密狗之间插入一个滤波器。硬件不存在了，剩下的就只有软件了。那只是 rtl_power [和这个奇妙的 GUI](http://sourceforge.net/projects/guiforrtlpower/) 。本教程使用廉价的 FM 滤波器，结果图显示在 50 至 150 MHz 之间有明显的下降。当然这不是很准确。没有任何衰减，无法与噪声源和转换器相比。这只是一个简单的问题，保存一些扫描。csv 文件和在 Excel 中插入一些数字。

同样的硬件可以用来确定天线的 VSWR，用定向耦合器代替滤波器；只需将耦合器放在噪声源和加密狗之间，测量加密狗范围内的衰减。在连接天线的情况下重复上述步骤，然后跳回 Excel。