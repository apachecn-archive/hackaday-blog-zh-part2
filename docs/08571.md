# 新零件日:SPI RAM 和视频控制器

> 原文：<https://hackaday.com/2015/03/18/new-part-day-spi-ram-and-a-video-controller/>

如果你没有注意到，用微控制器或旧 CPU 产生视频信号是很难的。如果你以每像素一位的速度驱动一个简单的 NTSC 或 PAL 显示器，你会发现至少有 64kB 左右的 RAM 被用作帧缓冲。大多数微控制器在芯片上没有这么多 RAM，我们看到的 AVR 视频版本要么[颜色糟糕](http://hackaday.com/2010/11/23/vga-interfacing-avr-microcontrollers/)要么[分辨率相对较低](http://hackaday.com/2013/03/29/avr-vga-generator/)。

[这里有个有趣的东西，解决了内存问题](http://www.vlsi.fi/en/products/vs23s010.html)，还能产生模拟视频信号。是的，这样的芯片是存在的，而且很明显这已经工作了很长时间。它是 VLSI VS23s010C-L，它有 131，072 字节的 SRAM 和支持 NTSC 和 PAL 输出的视频显示控制器。

该系列有两种芯片，一种是 LQFP48 封装，另一种是小型 SMD 8 引脚封装。从数据手册中我可以看出，8 引脚版本只是一个基于 SPI 的 SRAM 芯片。较大的 LQFP 封装是关键所在，它具有与存储器的并行和 SPI 接口、colorburst 晶体的输入、复合视频和同步输出。

[看了数据手册](http://www.vlsi.fi/fileadmin/datasheets/vs23s010.pdf) (PDF)后，看起来用这种芯片生成视频只是简单地连接一个 RCA 插孔，通过 SPI 向芯片发送几个命令，然后将位推入 SRAM。就是这样。你不会得到硬件加速，你将不得不一个像素一个像素地绘制一切，但这看起来是用单个部分生成相对高分辨率视频的最简单的方法。

感谢[antibyte]在这一点上的提示。