# 用开源硬件说话可以吗

> 原文：<https://hackaday.com/2015/03/28/speaking-can-with-open-source-hardware/>

你可以花 15 美元买到一个带有奇怪工业连接器的加密狗，它可以安装在路上任何汽车的仪表板下。这只是一个简单的 ODB-II 收发器，用于读取错误代码，并将皇冠 Vic 变成警方拦截器。CAN 总线不仅仅是 OBD-II；例如，机器人和工业控制单元，Hackaday alum [Eric] [开发了一个开源工具，可以用于所有事情](http://hackaday.io/project/579-cantact)。

[Eric]开发这个工具是因为缺少能说话的开源工具。有很多电路板可以在使用 OBD-II 的汽车中重置代码，但开放的硬件 can 设备并不真正存在。

[CAN act](http://cantact.io/)是一块小型电路板，一端配有 USB 端口，另一端配有 DE-9 端口，并且有足够的电子设备可以与任何 CAN 设备通信。CANtact 上的硬件是一个[STM 32 f 0](http://www.st.com/web/catalog/mmc/FM141/SC1169/SS1574/LN1823/PF259561)——一个带有 USB 和 CAN 接口的 ARM Cortex M0。这个芯片连接到一个[微芯片 CAN 收发器](http://www.microchip.com/wwwproducts/Devices.aspx?product=MCP2561)，这几乎就是你与汽车和工业自动化设备通话所需要的一切。如果你不喜欢用汽车中的 CAN 总线做一些合法、道德或安全的事情，那么 [Wired 报道你可以用数字技术切断某人的刹车线](http://www.wired.com/2015/03/60-gadget-thatll-make-car-hacking-easier-ever/)。

在软件方面，CANtact 可以与 Wireshark 和 [CANard](https://pypi.python.org/pypi/CANard/0.1.1) Python 库接口。所有的文件，从硬件到软件，[都可以在 Github](https://github.com/CANtact) 上找到。哦，坎塔克在[黑帽亚洲](https://www.blackhat.com/asia-15/briefings.html#hopping-on-the-can-bus)，这意味着【埃里克】在黑帽亚洲。我们应该给他寄贴纸的。