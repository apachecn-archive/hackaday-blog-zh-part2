# RTL-SDR 频谱分析仪

> 原文：<https://hackaday.com/2013/09/09/an-rtl-sdr-spectrum-analyzer/>

随着小型、强大、便携的计算机和廉价、现成的软件定义的无线电接收机的结合，有人用这些成分建造自制频谱分析仪只是时间问题。这个伟大的构建是[Stephen Ong]的项目，他甚至发布了所有的软件供你自己构建。

这款车的两个主要部件是一个比格犬骨黑色和它的 [7”触摸屏斗篷](http://circuitco.com/support/index.php?title=BeagleBone_LCD7)。BeagleBone 运行的是 [Angstrom Linux](http://www.angstrom-distribution.org/) ，这是一个用于小型嵌入式设备的速度惊人的 Linux 发行版。收音机硬件仅包括一个由 [RTL-SDR](http://sdr.osmocom.org/trac/wiki/rtl-sdr) 支持的 USB 电视调谐器。在他的[演示视频](http://www.youtube.com/watch?v=6YhrKMBrJ2g)中，【Stephen】展示了他的项目，从各方面来看，它都很出色，其用户界面比大多数面向桌面的 SDR 软件套件都要好。

你可以在他的博客上看到[Stephen]正在使用的 BeagleBone 图片，但是对于更有进取心的读者来说，他也把他的 ViewRF 软件的源代码放到了 GitHub 上。