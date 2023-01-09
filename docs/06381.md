# 用裸机汇编编程 Pi 游戏

> 原文：<https://hackaday.com/2014/06/23/programming-pi-games-with-bare-metal-assembly/>

虽然树莓 Pi 最常见的用途可能是媒体中心电脑或复古游戏模拟器，但 Pi *是*设计的教育电脑，旨在成为数百万学生手中易于使用的系统。伦敦帝国理工学院的 28 号团队无疑不负树莓 Pi 基金会的期望，用他们的裸机组装克隆了星狐，恰如其分地命名为 PiFox。

这不是大学课程第一次承担在没有操作系统的情况下为 Pi 开发软件的任务；几年前，剑桥大学开始为 Pi 开发一系列[裸机教程，包括在屏幕上绘制图形和摆弄 USB 键盘。PiFox 大大扩展了这些早期教程可以做的事情，从 GPIO 引脚读取 NES 操纵杆，使用 DMA 播放声音，以及渲染 3D 对象。](http://hackaday.com/2012/09/02/operating-systems-development-with-the-raspberry-pi/)

如果你想为自己构建 PiFox，或者更好，在现有的基础上扩展，[所有代码都在 Github](https://github.com/ICTeam28/PiFox) 上。还有[一个用于 Linux 的 Raspberry Pi 模拟器](https://github.com/ICTeam28/PiEmu)，以防万一你有一个你不能用 Raspberry Pi 抓的 ARM 装配 bug。

[https://www.youtube.com/embed/-5n9IxSQH1M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-5n9IxSQH1M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)