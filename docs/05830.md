# 嗅探自动售货机公共汽车

> 原文：<https://hackaday.com/2014/04/18/sniffing-vending-machine-buses/>

我们已经讨论了各种协议以及如何处理它们。今天，【丹】正在研究[嗅探自动售货机多点总线](http://www.marginallyclever.com/blog/2014/04/making-sense-of-vending-machine-multidrop-bus-communications/)。[多点总线](http://en.wikipedia.org/wiki/Multidrop_bus) (MDB)协议是自动售货机中使用的一种标准，用于将货币收集器等设备连接到主机控制器。

要连接到总线，需要接口硬件。[Dan]设计出兼容的硬件并将其连接到 Arduino 上。有了总线上的设备，[Dan]开始研究 Arduino 草图，将 MDB 数据解析成人类可读的格式。通过这种方式，可以很容易地在 Arduino 的串行控制台上发现总线。

这只是一个更复杂项目的开始。由于该协议用于与自动售货机的货币收集器或读卡器进行通信，因此能够进行通信将允许他实现自己的支付方法。该计划旨在扩大他在温哥华 Hack Space 经营的[自动售货机，以接受比特币。我们期待着看到那个项目的展开。](http://vancouver.hackspace.ca/wp/tag/vending-machine/)