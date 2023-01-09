# 基于英特尔技术的 Arduino

> 原文：<https://hackaday.com/2013/10/03/the-intel-powered-arduino/>

基于微控制器和 ARM 片上系统的开发板随处可见，但要找到一台基于英特尔处理器的小型便携式计算机却很难。Arduino 的[Massimo]刚刚在罗马 Maker Faire 发布了一款新的英特尔架构 Arduino 兼容主板。它被称为 Galileo ，它拥有你所期望的运行 x86 的 Arduino 的一切。

主芯片是一个运行频率为 400MHz 的英特尔 Quark SoC，具有 256 MB 的 DRAM。板上有一个迷你 PCIe 插槽、100Mb 以太网端口、微型 SD 插槽、RS-232 以及 USB 主机和客户端端口。[这是 Galileo 的数据表](https://communities.intel.com/docs/DOC-21831)，包含所有适用的信息。

Galileo 可以使用标准的 Arduino IDE 进行编程，但是从[入门指南](https://communities.intel.com/docs/DOC-21832)来看，这款主板似乎正在运行 Yocto，这是一款针对嵌入式环境的精简版 Linux。

实际上，我们现在拥有的是一个处理能力与 Raspberry Pi 相当的*板，但是兼容 Arduino，以及一个用于一些真正有趣的东西的迷你 PCIe 端口。看看这个板能做些什么会很有趣，但是如果你在 Galileo 两个月后发布之前有什么想法，请在评论中留言。*