# 通过 USB 并行端口适配器的位碰撞

> 原文：<https://hackaday.com/2013/02/21/bit-banging-through-a-usb-parallel-port-adapter/>

如果您曾经研究过低级并行端口访问，您可能已经知道它只适用于实际的并行端口硬件，而不适用于 USB 并行端口适配器。但是这里有一个解决方案会改变你的想法。它借鉴了打印机通信的方式，允许 [USB 到并行端口位碰撞，而无需微控制器](http://www.ccs.neu.edu/home/bchafy/parallel/parallel.html)(死链，试试[互联网存档](http://web.archive.org/web/20130226141444/http://www.ccs.neu.edu/home/bchafy/parallel/parallel.html))。

当然，增加一个微控制器会让这变得非常简单。你所需要做的就是对芯片进行编程，以模拟打印机端的通信方案。但这不是这里采用的方法。相反，上图中的 USB 转 RS232(串行)转换器用作复位信号。并行端口上的 strobe 引脚驱动一个反相器，该反相器触发连接到 busy 引脚的晶闸管。晶闸管是双稳态开关，因此仅靠这种解决方案永远无法清除 busy 引脚。这就是串行连接发挥作用的地方。通过在发送至 LP0 的 bit-bang 值和发送至串行连接器的 0xF0 值之间交替传输来自计算机的数据，8 个并行数据位变得完全可寻址。休息后，在剪辑中查看项目的运行情况。