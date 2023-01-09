# 完整的 C64 系统，在 STM32 上仿真

> 原文：<https://hackaday.com/2014/10/23/a-complete-c64-system-emulated-on-an-stm32/>

Commodore 64 是世界上最畅销的电脑，我们非常确定大多数超过一定年龄的程序员和工程师至少将他们职业生涯的一部分归功于这个棕色/米色键盘，它也是一台电脑。这些工程师现在都长大了，也该来几个翻拍了。[Jeri Ellisworth]将她的成功归功于她的版本，有无数片 C64 电路漂浮在各种微控制器周围，现在[Mathias]已经在单个 ARM 微控制器中模拟了一切(除了 SID，那仍然是黑魔法)。

在项目页面上，[Mathais] [介绍了他的董事会](http://www.staringlizard.com/index.php/projects/3-memwa#hardware)的能力。它使用 STM32F4，超频到 235 MHz。有一个用于 7 英寸 800×480 TFT 的显示控制器，以及用于 C64 游戏库的 4GB 内存。如果没有显示屏，整个项目就比一张名片大一点。有了显示器，它实际上是一个 C64 平板电脑，不包括键盘。

这是对 C64 的直接模拟，直到原始版本的 6510 CPU 中的单个操作码。原始系统中的一切都是仿真的，从 VIC、CIA 和 VIAs、串行端口，甚至 1541 磁盘驱动器的 CPU。唯一没有被仿真的是 SID 芯片。那块珍贵的芯片坐落在 ZIF 插座上，让旁观者大为惊讶。

你可以在这里查看一些图片，或者下面的视频演示。

[https://www.youtube.com/embed/uI4o9XAFLt0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uI4o9XAFLt0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)