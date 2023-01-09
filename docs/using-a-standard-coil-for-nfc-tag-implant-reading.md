# 使用标准线圈进行 NFC 标签植入读取

> 原文：<https://hackaday.com/2014/10/08/using-a-standard-coil-for-nfc-tag-implant-reading/>

几个月前，Hackaday 报道了 xNT 众筹活动，该活动旨在制造一种基于 NTAG216 的 NFC 植入物，用于不同目的。我实际上支持它，发现标准的 NFC 读取器性能不佳，因此决定尝试使用标准线圈作为天线，以获得更好的读取性能。

大多数 NFC 读卡器通常只有一个小的最佳点，可以读取植入物。这是由于我们所谓的*耦合系数*，它取决于读取距离和读取器& NFC 标签天线的几何形状。天线直径越小，耦合系数越大，植入定位越容易。

在我的详细文章中，您会发现对阻抗匹配有一个很好的介绍，在这个过程中，一些无源元件与天线串联/并联，使其复阻抗接近 RF 信号发射器的复阻抗。这通常需要昂贵的工具，但允许在给定频率下的最佳功率传输。

你可以在这里找到我们 xNT 的报道[。](http://hackaday.com/2013/10/30/hackaday-interview-with-amal-graafstra-creator-of-xnt-implant-chip/)