# 对机械臂进行逆向工程

> 原文：<https://hackaday.com/2014/12/15/reverse-engineering-a-robotic-arm/>

没有太多人会认为机器人手臂不酷。[Dan]认为他们很酷，在易贝花了 150 美元买了一个 LabVolt Armdroid 机械臂。不幸的是，他没有得到电源或控制单元。对大多数人来说，这是一个需要克服的严重障碍，但对[丹]来说不是。他打开机器人，开始在电路板周围探测，想弄清楚发生了什么。

由于在机器人手臂的外部有一个 DB9 连接器，他认为这是一个标准的 RS-232 控制的设备。还好他检查了内部电路，因为根本不是这样。里面没有微型控制器或微处理器。[Dan]煞费苦心地对电路板进行逆向工程，[记录了他的结果](http://dankohn.info/projects/armdroid_1000/schematic.pdf)。他发现有 [SN76537A 芯片](http://www.ti.com/lit/ds/symlink/sn75437a.pdf)驱动 6 个单极步进电机和 [SN75HC259](http://www.ti.com/lit/ds/symlink/sn74hc259.pdf) 锁存器来寻址每个单独的电机。

现在知道了机器人是如何工作的，[丹]必须想出如何从他的电脑控制机器人。他首先制作了一个定制的[并行端口到 DB9](http://dankohn.info/projects/armdroid_1000/wiring.pdf) 电缆，将计算机连接到手臂上。在一系列的几个程序之后，从简单地移动一个手臂关节开始，[最新的迭代](http://dankohn.info/projects/armdroid_1000/armdroid_5.asm)允许使用计算机键盘手动控制所有关节。非常感谢[Dan]所做的工作和文档。