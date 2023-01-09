# 使用 Linux 进行实时任务的教程

> 原文：<https://hackaday.com/2014/04/25/a-tutorial-on-linux-for-real-time-tasks/>

[Andreas]创建了这个关于 Linux 中实时(RT)任务的教程。乍一看，这听起来像是一个相当枯燥的话题，但[Andreas]通过使用树莓 Pi 和步进电机给我们一些真实世界的演示，让事情变得有趣起来。驱动步进电机需要相对精确的定时。试图使用桌面操作系统来完成这样的任务通常是不明智的。精确计时最好留给独立的微控制器。这就是为什么我们经常在 Hackaday 上看到 [Raspi 和 Arduino](http://hackaday.com/2012/11/16/raspberry-pi-driven-polargraph-exhibits-high-precision-drawing-ability/) 配对。这背后的基本原理并不经常被解释。

[Andreas]将带有 ULN2003 驱动板的普通低成本 28BYJ-48 齿轮步进电机连接到 Raspberry Pi 的 GPIO 引脚。这些马达最初用于移动空调的百叶窗。总的来说，他们完成了工作，但是质量不高。[Andreas]使用一个简单的程序以正确的顺序脉冲引脚来旋转电机。使用示波器、分屏显示器和步进电机上的摄像头，[Andreas]向我们展示了几种常见的时序危险，以及如何避免它们。

最明显的危险出现在最后。在运行他的步进程序时，[Andreas]运行第二个分配大量内存的程序。最终，Linux 交换了步进程序的内存，导致步进电机停止旋转几秒钟。不过，并没有全部丢失，因为可以通过 mlockall()调用来防止交换。

由此得出的结论是，Linux 不是一个硬实时操作系统。通过一些技巧和扩展，它可以完成一些软实时任务。最佳解决方案是要么使用为实时操作设计的[操作系统，要么将实时操作卸载到单独的控制器。](http://en.wikipedia.org/wiki/List_of_real-time_operating_systems)

[https://www.youtube.com/embed/uIXkvz1-weQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uIXkvz1-weQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)