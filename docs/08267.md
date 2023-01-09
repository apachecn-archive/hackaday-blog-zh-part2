# Raspberry Pi 2 的光子重置

> 原文：<https://hackaday.com/2015/02/08/photonic-reset-of-the-raspberry-pi-2/>

在过去的一个月里，Raspberry Pi 2 只对 Raspi 基金会开放，在大约 2 周的时间里，选择那些将 Raspi 2 戴在项链上的媒体成员，如[Flavor Flav]戴着一个时钟。没有多少人拥有真正的、可以工作的硬件，当一个产品发布的时候，大量没有洗过手的人会发现一些非常非常奇怪的 bug。[首先出现的是 Raspberry Pi 2 的光敏复位](http://www.raspberrypi.org/forums/viewtopic.php?f=28&t=99042)。

[PeterO]在 Raspberry Pi 论坛上用闪光灯拍了几张运行中的 Raspberry Pi 2 的照片。经过一点推理，我们才意识到相机闪光灯要么会重置，要么会关闭 Raspi 2。是的，这很奇怪，实验正在进行中。

[来自【迈克·雷德罗布】](https://www.youtube.com/watch?v=c7p2OcQ7G58)的一个短视频证实了这一发现，[一个 reddit 帖子](https://www.reddit.com/r/linux/comments/2v6kwm/raspberry_pi_a_xenon_flash_will_cause_the/)给出了解释。U16 是位于 Raspi 2 电源部分的一个小芯片，对光很敏感。放入足够的光子会导致 Pi 关闭或重启。

还有一些研究要做，不过， ***我可以确认一个便宜的绿色激光笔会在光束对准 U16 芯片的时候重置一个树莓 Pi 2*T3。这是芯片的责任，这不是电磁脉冲的问题。这是 U16 芯片的光子/光问题。解决这个问题的方法是要么把它放在一个盒子里，要么在芯片上贴一点点绝缘胶带。**

感谢[Arko]熬夜到一个邪恶的小时，并发送给我这个。