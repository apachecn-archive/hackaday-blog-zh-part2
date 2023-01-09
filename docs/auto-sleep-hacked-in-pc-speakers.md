# 电脑扬声器的自动睡眠被黑

> 原文：<https://hackaday.com/2015/03/19/auto-sleep-hacked-in-pc-speakers/>

我们可以同情那些不愿意让电脑扬声器一直开着的人。当你把音量旋钮转到最低档直到发出咔嗒声时，他使用的创造性的 T20 装置就关闭了。所以关掉它们意味着每次它们再次打开时都要重新定位音量。这种黑客技术通过[自动开启和关闭](http://morethanuser.blogspot.com/2015/03/creative-t20-speakers-stanby-mode.html)而无需触摸旋钮，一举两得。

该系统基于 ATtiny45 和其他一些简单的组件。它使用两个 ADC 来监控电脑扬声器的后置输入通道。如果超过一分钟没有检测到声音，扬声器 amp 芯片的 shutdown 引脚将被触发。这还不是黑客攻击的终点。我们提到它监控扬声器的后置输入，但它不监控前置辅助输入。使用此前端输入时，另一个按钮用于禁用自动睡眠。当扬声器睡眠时，LED 上还有一个基于 PWM 的心跳。

[HardwareCoder]担心我们不会对此感兴趣，因为它与我们几年前的一次黑客攻击非常相似。我们希望你会同意它值得再看一眼。他还警告我们演示视频很无聊。不管怎样，我们都看了，可以确定那里没有太多的动作，但是我们还是把它嵌入了下面。

[https://www.youtube.com/embed/BxWnkHDRhuI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/BxWnkHDRhuI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)