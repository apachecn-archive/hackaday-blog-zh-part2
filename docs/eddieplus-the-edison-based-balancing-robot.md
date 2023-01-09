# 埃迪普勒斯，爱迪生公司的平衡机器人

> 原文：<https://hackaday.com/2015/02/24/eddieplus-the-edison-based-balancing-robot/>

[Renee]给了我们一个提示，让我们了解她的平衡机器人创作 [EddiePlus。](http://www.thingiverse.com/thing:694969)顾名思义，EddiePlus 由英特尔 Edison 处理器控制。更具体地说，[蕾妮]正在用 Sparkfun 的几个[爱迪生积木](https://www.sparkfun.com/categories/272)来创造埃迪的大脑。EddiePlus 的身体是 3D 打印的，而他的运动来自两个带轮子和编码器的 Pololu DC 电机。完整的构建说明可以从[Renee 的]Google drive 中以[PDF 格式获得。](https://drive.google.com/file/d/0B0pRXCySIopjcWRlSXN6NmRXdG8/view?usp=sharing)

埃迪能够在两个轮子上平衡和驾驶，很像赛格威。用于平衡的传感器数据来自 Sparkfun 基于 LSM9DS0 的惯性测量单元(IMU)模块。在这个新的“增强版”埃迪中，[雷尼]在机器人的轮子上增加了编码器。这让他更容易适应变化的负载——比如抽熨斗(或者香蕉插头，视情况而定)。编码器也有助于改变地形，正如[Renee]通过 Eddie 在上面驾驶时倾斜一块板所展示的那样。Eddie 的代码是用 C 写的，可以在 [Github 上找到。](https://github.com/r3n33)控制 Eddie 就像通过 UDP 发送简单命令一样简单。

正如你可能想象的那样，在计算埃迪的平衡后，英特尔爱迪生仍然有很多周期。[Renee]将其中一些与基于网络摄像头的远程操作模式结合使用。

点击过去的休息，看看埃迪在行动！

[https://www.youtube.com/embed/2_HegEclIyQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/2_HegEclIyQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/LNMD3ySDc_8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LNMD3ySDc_8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/1JDhUngas1Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1JDhUngas1Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)