# WSPR 发射机展示了树莓 Pi 对黑客攻击的真正价值

> 原文：<https://hackaday.com/2013/03/21/wspr-transmitter-shows-true-value-of-raspberry-pi-for-hacking/>

![wspr](img/ef486d6b04bf3ab3aaa30f378041b861.png)

别误会，我们爱我们的树莓派。但是，如果你只是运行一个 Linux 映像，而没有添加硬件插件，你就错过了开发这个平台的部分功能。这个项目是一个很好的例子，展示了如何利用 Raspberry Pi 的能力来提供底层硬件访问和稳定的嵌入式 Linux 性能。[Dan Ankers]和[Threeme3]开发了一个程序，将 RPi 转化为 WSPR 发射器。GitHub readme 分享了许多关于它是如何完成的细节。但是你也会想挖掘。c 文件，看看他们是如何利用 GPIO 头引脚的。

[William Meara]发来了这个的消息。他之前曾因 WSPR (弱信号传播报告)的工作而在 Hackaday 上被特写。这是一种业余无线电协议，它允许你使用相对较弱的发射机进行远距离通信。诀窍是利用计算能力找到隐藏在所有噪音中的信号。请注意，您确实需要一个 HAM 许可证来尝试这一点，但除此之外，您需要连接到电路板的只是一个低通滤波器和一个天线。

[通过[焊烟](http://soldersmoke.blogspot.com/2013/03/wow-raspberry-pi-as-rf-transmitter.html)

[图片来源: [WSPR 主页](http://physics.princeton.edu/pulsar/K1JT/wspr.html)