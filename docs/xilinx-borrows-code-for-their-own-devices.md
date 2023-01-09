# Xilinx 为他们自己的设备借用代码

> 原文：<https://hackaday.com/2015/05/12/xilinx-borrows-code-for-their-own-devices/>

早在 2012 年，[tmbinc]就在 Xilinx ISE 中发现了[一个巧妙的未记录的小功能:使用 TCP/IP 代替 JTAG 电缆的能力。[tmbinc]正在开发一个开放式硬件 USB 分析器，并发现了几乎没有文档记录的 Xilinx 虚拟电缆，这是一个单独的“shift”命令，可以打开 TCP 连接，并将 JTAG 数据发送到网络上的另一台计算机。它非常有用，【tmbinc】](http://debugmo.de/2012/02/xvcd-the-xilinx-virtual-cable-daemon/)[为这个工具](https://github.com/tmbinc/xvcd)写了一个守护进程，一切正常。

昨天，[tmbinc] [再次发现了 Xilinx 虚拟电缆](https://github.com/Xilinx/XilinxVirtualCable/issues/1)，这次是在 Xilinx 的 Github repos 之一。这段代码非常熟悉，仔细查看了几处修改后，他发现这段代码与他三年前写的代码非常相似。

Xilinx repo 中令人不快的[版本与](https://github.com/Xilinx/XilinxVirtualCable/commit/eae2da80c4ad4ff22083d88ab1aa2dad46fc3bc9)[【tmbinc】的 Xilinx 虚拟电缆驱动程序守护进程](https://github.com/tmbinc/xvcd/blob/master/src/xvcd.c)几乎相同。变量名是相同的，变量以相同的顺序声明，除了空格，代码约定是相同的。这并不是说 Xilinx 有人从[tmbinc]窃取代码，但如果这是一个计算机科学实验室，就会有一场学术纪律听证会。更糟糕的是，Xilinx [把他们的版权声明贴在代码](https://github.com/Xilinx/XilinxVirtualCable/blob/master/XAPP1251/xvcServer.c)的顶部。

在[tmbinc]提出的一个问题中，他说他很荣幸，但澄清说他的代码完全是从头开始开发的。他认为 Xilinx 代码源自他自己三年前写的代码。由于[tmbinc]的代码是在没有许可证的情况下上传的，因此默认保留所有权利。这对 Xilinx 法律部门来说不是一个好兆头。

在任何情况下，你真的真的想知道 Xilinx 的内部文档是什么样子的，如果互联网上的一个随机的人可以发现一个几乎没有记录的协议，编写一个守护程序，把它放在互联网上，并让 Xilinx 的某人使用该代码。

感谢匿名举报人将此信息发送到黑客日小费罐。