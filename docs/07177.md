# 复活飞利浦 HDD 1420 MP3 播放器

> 原文：<https://hackaday.com/2014/09/26/reanimating-a-philips-hdd-1420-mp3-player/>

[OiD]有一个满是灰尘的，旧的，被遗忘的飞利浦 HDD1420 GoGear mp3 播放器在他的地方踢来踢去。你可以想象，电池没电了。他没有充电器或连接器，但[决定无论如何都要让它复活](http://figuramania.blogspot.com.es/2014/09/hacked-up-usb-for-phillips-hdd1420.html)。

他认为这只是提供替代电源的问题，但 GoGear 没有，坚持要连接到计算机上。他很幸运地查阅了 Pinouts.ru 并找到了飞利浦自己的设备管理软件，但这仍然不容易。设备管理器在 Windows 7 上不工作。他试了一个 XP 盒子，但是没有检测到设备。

最后，他发现硬盘坏了，换了一个 8GB 的微硬盘。这很有帮助，但他仍有一大堆工作要做。[OiD]格式化了新的 HD，并给了它官方固件，但仍然必须根据飞利浦手册替换一些系统文件。他最终使用 [RockBox](http://www.rockbox.org/wiki/GoGearHDD6330) 将其复活，并决定将它保留在设备上。

不过，充电还是有问题。它有一个 IC 来处理专有外部适配器或 USB 电源的选择，但 RockBox 固件不实现切换，默认为适配器。几个调整和一个黑客入侵的迷你 USB 后，病人的情况稳定，并开始播放音乐。