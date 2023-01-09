# 基于 Hackaday 开发:安全性和 Arduino 兼容性

> 原文：<https://hackaday.com/2014/03/16/developed-on-hackaday-security-and-arduino-compatibility/>

[![2013-12_Developed_on_Hackaday](img/4126eb698213947e5ac36e95f300751f.png)](http://hackaday.com/wp-content/uploads/2013/12/2013-12_developed_on_hackaday.png)

我们的一些读者注意到，Hackaday 社区开源离线密码管理器(又名 [Mooltipass](http://projects.hackaday.com/project/86-Mooltipass) )有两个不兼容的特征:安全和 Arduino 兼容。

这是为什么呢？Arduino 兼容性意味着包括改变设备固件和访问微控制器引脚以连接屏蔽的方法。因此，一些居心不良的个人可能会用记录所有用户输入和密码的固件来替换原始固件，或者在另一种情况下，只是嗅探 uC 的信号。“黑客”随后会提取记录的数据。因此，我们需要一个安全防篡改的 Mooltipass 版本和一个 Arduino 兼容版本，同时允许前者成为后者。

Olivier 的设计虽然是完全封闭的，但在 Arduino 头上方会有几个更薄的表面。作为一种妥协，我们因此想到向只对密码管理器功能感兴趣的人发送一个无引导装载程序的组装版本，而向修补者发送一个非组装版本(带有预刻录的引导装载程序)。Arduino 爱好者只需要在关键的地方切割塑料(也许焊接头部以节省成本)。这样做的主要优点是两个版本的情况是相同的。缺点是每块板都有不同的固件，这取决于它的目标用户。

我们的读者怎么想？关于 Mooltipass 当前状态的更多详细更新，您可以随时加入[官方 Google 群组](https://groups.google.com/forum/?hl=en#!forum/mooltipass)。