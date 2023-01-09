# 通过 CAN 总线控制 Choo-Choo 的路由器

> 原文：<https://hackaday.com/2012/06/17/router-controlling-choo-choos-over-the-can-bus/>

该设置用于控制模型铁路。嗯，不完全是这样。[Gerhard Bertelsmann]已经有了一个合适的铁路控制器，它正好提供 CAN 总线通信。他正在使用 OpenWRT 和一个便宜的路由器将总线连接到网络。

最初他想为这个项目使用一个 Raspberry Pi 板，但是令人难以置信的硬件缺货情况导致他使用了一个旧路由器。加载 OpenWRT 后，他开始研究如何连接几个负责 CAN 总线通信的 IC(MCP 2515 和 MCP2551)。硬件连接非常简单，五条数据线(及其上拉电阻)连接到路由器的串行接口。接下来就是在软件中映射设备，以便可以通过网络控制硬件。

我们喜欢这个例子，因为 CAN 还用于许多其他应用。