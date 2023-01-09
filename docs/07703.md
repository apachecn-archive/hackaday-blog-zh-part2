# 在 Arduino 上使用第二个微控制器

> 原文：<https://hackaday.com/2014/11/30/using-the-second-microcontroller-on-an-arduino/>

而较新的 Arduinos 和 Arduino 兼容机([包括 Hackaday.io Trinket Pro。超级犯罪广告](http://store.hackaday.com/products/trinket-pro-with-black-solder-mask-and-the-hackaday-io-logo)！)要么有一个支持 USB 的芯片，要么依靠 V-USB 实现，Arduino 世界的老古董 Uno 和 Mega 实际上有两个芯片。ATMega16u2 负责 USB 连接，而标准的' 328 或' 2560 负责所有 duino 任务。如果您还可以使用 Uno 或 Mega 上的 16u2 为您的 Arduino 草图添加一些附加功能，那岂不是很棒？[这是现在的现实。](https://github.com/NicoHood/HoodLoader2) [Nico]已经在 HoodLoader2 上工作了一段时间，当前版本让您可以选择用自定义草图重新编程 16u2，并在这个以前被忽略的芯片上使用 7 个 I/O 引脚。

与以前的 HoodLoader 不同，这个版本是一个真正的 16u2 引导加载程序，它用 CDC 引导加载程序和 USB 串行功能取代了 DFU 引导加载程序。这允许新的 USB 功能，如 HID 键盘、鼠标、媒体键和游戏手柄，添加额外的传感器或 led，以及其他任何你可以用普通“duino”做的事情。

设置非常简单，只需要在 328 ISP 接头和 16u2 接头上的引脚之间进行连接。在[Nico]的博客上已经有一些关于 16u2 的新固件能做什么的示例，但我们预计使用这个新引导程序的示例项目的数量将在未来几个月内激增。如果您曾经参加过 Arduino Demoscene 竞赛，并且您正在寻找更多的引脚和代码空间，现在您知道去哪里找了。