# 没有电脑流光溢彩克隆使用电脑

> 原文：<https://hackaday.com/2013/08/05/no-computer-ambilight-clone-uses-a-computer/>

当这个黑客是关于[一个不需要计算机](https://github.com/gkaindl/ambi-tv)的流光溢彩克隆系统时，你看到的是树莓派，这可能看起来令人困惑。这里的要点是，无论你的视频源是什么，这个系统都可以工作，过去的许多项目都要求视频从计算机上播放。

这次攻击遵循了我们大约一个月前的基于 ARM 的定制任务的相同路线。就像那个项目一样，你使用一个 HDMI 分路器来接入你的电视。分离信号馈入 HDMI 转复合视频适配器。复合信号由 USB 视频编码器捕获。GPIO 接头驱动一条可寻址的 RGB LEDs。整件事是作为一个使用一点电缆黑客供电。

有点复杂。但是所有的部件都很容易获得并且相对便宜。一个警告是，如果你已经在使用硬件 HDMI 源选择器，而不是内置在你的电视上，它的效果最好。这样，只有一根 HDMI 电缆连接到电视，这样就可以从电视信号中抽取信号。

[https://www.youtube.com/embed/8cpQpGYtjR0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8cpQpGYtjR0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)