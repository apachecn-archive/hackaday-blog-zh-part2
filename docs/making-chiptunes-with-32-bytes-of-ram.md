# 用 32 字节的 RAM 制作芯片调谐器

> 原文：<https://hackaday.com/2012/08/14/making-chiptunes-with-32-bytes-of-ram/>

[https://player.vimeo.com/video/47380710](https://player.vimeo.com/video/47380710)

啊，小甜饼。这是人类所做的为数不多的努力之一，在这些努力中，更少的内存、更少的存储空间和更少的功能实际上被认为是一种改进。斯图加特 hackerspace Shackspace 送来了一个小小的 chiptune 游戏电路，使用了我们见过的最简单的硬件。

Noiseplug，如[dop3joe]所称，是基于一个非常非常小的 6 针。凭借 1 kB 的闪存和仅 32 字节的 RAM ,[ dop3 Joe]能够在 RCA 插孔内创建一个小型设备，每当它由电池供电时，就可以播放 chiptunes。

如果你想做自己的噪音插件，[dop3j0e]把所有代码[放到他的 Git](https://github.com/dop3j0e/noiseplug)里。这个版本有两个相关的软件:一个创建 chiptunes 的 Windows 应用程序和 ATtiny9 固件本身。当然，要对 tiny 编程，你必须处理 Atmel TPI，所以[这是应用笔记](http://www.atmel.cimg/doc8373.pdf) (PDF)。

哦，【dop3 Joe】[凭借 Noiseplug 在上周末的](http://shackspace.de/?p=3352)[唤起民众派对](http://www.evoke.eu/2012/)上获得第三名。太棒了。