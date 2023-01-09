# 采访 9 美元单板机芯片的创造者

> 原文：<https://hackaday.com/2015/05/19/interview-with-the-creators-of-chip-a-9-single-board-computer/>

单板计算现在是 DIY 领域的热点，而骑在刀刃上的是 C.H.I.P .，一个目前正在众筹的项目，其基本单元的价格仅为 9 美元。我很高兴遇到了 Next/Thing Company 的工作人员，他们开发了 C.H.I.P。他们很高兴，因为这个项目的反响就像一颗超新星。目前，他们离最初的 5 万美元目标大约还有 150 万美元。我们谈到了在板上运行 Linux，有哪些连接器和引脚排列头可用，以及他们为板准备的各种外设硬件。

[https://www.youtube.com/embed/GT-y3GnDQp4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/GT-y3GnDQp4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

## 9 美元，但是…

上周我发表了一篇文章[讨论 Linux 发展成为主流](http://hackaday.com/2015/05/08/c-h-i-p-is-a-linux-trojan-horse-for-nine-bucks/)的可能性，因为工程师们是伴随着 C.H.I.P、Raspberry Pi、BeagleBone Black 等主板成长起来的。当时我在想，这些主板中的大多数将被用作台式计算机。我的想法有所改变(稍后我会谈到这一点)，但我认为值得注意的是，大多数人不会为此使用 9 美元的基本模式。它只配有复合视频。所以关于价格的“但是”是你需要为 VGA 或 HDMI 适配器多花 10-15 美元。正如我之前所说，这不是一个交易破坏者。

亲自看过之后，我开始怀疑这是否会被用于许多无头项目？

## …是啊，也许只要 9 美元

有很多理由可以让它成为完全不需要显示器的项目，这样可以节省未使用端口的电路板空间或 BOM 成本。

它内置了电源管理(X-Powers AXP209 PMIC 芯片)，便于操作和电池充电。有 WiFi 和蓝牙，摄像头支持，8 GPIO，和你的标准 UART/SPI/I2C。想想所有相对繁重的嵌入式项目都在乞求这种马力和价格:漫游者、无人机和可视化显示器(想想[巨大的 LED 矩阵](http://hackaday.com/2015/04/17/1768-leds-because-96-just-wasnt-enough/)或[巨大的翻转点显示器](http://hackaday.com/2015/01/14/the-giant-flip-dot-display-at-ces/)等等。当我能得到其中一个的时候，我会有兴趣去探索 GPIO 的延迟；我们听说过的一个关于 Raspberry Pi 供电设备的问题。

## 你可以带着它

我不太确定该怎么看待这个袖珍的加州公共卫生研究所。

这是一款便携式机型，拥有巨大的屏幕和全键盘。基本单元插入背面，在一个有趣的几何形状的箱子里面(任何东西都比矩形好，对吗？).当然，这一切都靠电池运行。

我没有看到自己使用这样的东西，但我显然不是目标人群。在智能手机时代，很难想象有什么东西不是非常便宜的。另一方面，仅仅将参考设计作为您可以围绕基本单元构建的示例，对他们来说就是一个很好的营销举措。“嘿，看这个 PCB 上的 ARM 芯片”——嗯。“嘿，看看这个 ARM-board 为一台带有 clicky 键盘的便携式触摸屏计算机提供动力”——太棒了！