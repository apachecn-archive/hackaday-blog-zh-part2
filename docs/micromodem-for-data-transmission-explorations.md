# 微型调制解调器，用于数据传输探索

> 原文：<https://hackaday.com/2014/05/15/micromodem-for-data-transmission-explorations/>

那些戴着 Arduinos 的孩子不知道他们错过了什么。串行连接太简单了，而且使用低带宽调制解调器有很多乐趣。考虑到这一点，马克制作了微型模型 T2。这是一个 1200 波特的 AFSK 调制解调器，能够进行 APRS、TCP/IP over SLIP、网状网络实验，甚至远程无线电通信。

由于 MicroModem 旨在引入数字无线通信，因此它非常简单，仅使用与 [Microduino](http://microduino.cc/) 兼容的电路板上的 17 个组件。该软件是围绕一种名为 MinimalProtocol1 的协议构建的，该协议将被所有其他监听站接收，具有纠错和自动数据压缩功能。还有通过链接发送 TCP/IP 的能力，这允许[马克]以 1200 bps 的速度加载[我们的复古网站](http://retro.hackaday.com/)。

代码被很好地记录下来，如这个项目的 Github 上的[所示，包括电路板文件，甚至包括试验板布局。[Mark]还有三块他原型的 PCB，他愿意把这些给其他想试试他的调制解调器的 Hackaday 读者。](https://github.com/markqvist/MicroModem)