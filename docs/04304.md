# CAN 黑客:简介

> 原文：<https://hackaday.com/2013/10/21/can-hacking-introductions/>

我们将推出一个关于 CAN 和汽车黑客的新系列。首先，我们将介绍 CAN 并讨论车载网络的工作原理。

1986 年，博世推出了控制器局域网协议。它是专门为汽车控制器之间的车载网络而设计的。CAN 成为汽车、工业和机器人应用中网络控制器的流行选项。从 2008 年开始，在美国销售的所有车辆都必须使用 CAN。

现代车辆是分布式控制系统，控制器设计用于处理特定的任务。例如，门控制模块将负责锁和窗户。CAN 允许这些控制器进行通信。它还允许外部系统通过连接到车载网络来执行诊断任务。

车辆中 CAN 通信的一些示例包括:

*   发动机控制模块将当前发动机转速发送至组合仪表，并显示在转速表上。
*   驾驶员车门控制器向另一个车门控制器发送信息以启动车窗。
*   从诊断工具发送的控制器固件升级。

除了通信的模糊性，CAN 通常很少或没有安全性。我们可以使用 can 转 USB 接口监听流量，然后解码。我们还可以使用这些工具发送伪造的消息，或者执行诊断操作。不幸的是，大多数处理 CAN 的工具都是专有的，而且非常昂贵。诊断协议是标准的，但不是开放的。它们必须从国际标准化组织购买。

下一次，我们将探讨 CAN 帧的结构，以及总线上的流量是如何编码的。

[图片来自[维基百科](http://en.wikipedia.org/wiki/File:CAN-Bus-frame_in_base_format_without_stuffbits.png)

## 可以黑客攻击

*   [介绍](http://hackaday.com/2013/10/21/can-hacking-introductions)
*   [车载网络](http://hackaday.com/2013/10/22/can-hacking-the-in-vehicle-network/)
*   [CAN 协议](http://hackaday.com/2013/10/29/can-hacking-protocols/)
*   [建筑 CAN 硬件](http://hackaday.com/2013/11/05/can-hacking-the-hardware/)