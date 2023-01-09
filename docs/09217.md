# 入侵即时通讯软件打开车库

> 原文：<https://hackaday.com/2015/06/08/hacking-the-im-me-to-open-garages/>

如果你有一个无线控制的车库门，孩子的玩具可以在几秒钟内无线打开它。【Samy Kamkar】是一个喜欢“往坏处想，往好处做”的安全研究员。他利用他在无线固定密码设备中发现的一种新攻击，利用 Mattel IM-ME 玩具，开发了一种可以在几秒钟内无线打开几乎任何固定密码车库门的设备。

该漏洞只对使用“固定代码”的大门或车库有效。为了防止这种类型的攻击，你需要做的就是升级到一个使用滚动码、跳跃码、安全+或智能码的系统。这些都不是绝对安全的，但是可以防止 OpenSesame 攻击和其他传统的暴力攻击。看起来至少有几家厂商仍然有这样易受攻击的产品，还有几家厂商的旧版本也受到了影响。

在你进一步阅读之前，有一个警告——由[Samy]发布的代码被有意地屏蔽，以防止它被滥用。它可能会起作用，但不完全是这样。如果你是射频和微控制器方面的专家，你可以修好它，但是你首先就不需要他的帮助了，对吗？

IM-ME 是一个废弃的玩具，Mattel 不再生产它，但如果你幸运的话，它可以在亚马逊或易贝买到。Radica Girltech IM-ME 短信玩具已经被大量黑客攻击和记录在案。这并不奇怪，因为它配备了一个 [TI CC1110](http://www.ti.com/product/cc1110-cc1111) 亚 GHz 射频芯片、一个 LCD 显示屏、键盘、背光等等。一个很好的起点是 [GoodFET](http://goodfet.sourceforge.net) 开源 JTAG 适配器，然后是 [Travis Godspeed](http://travisgoodspeed.blogspot.in/2010/03/im-me-goodfet-wiring-tutorial.html) 、 [Dave](http://daveshacks.blogspot.in/2010/01/im-me-hacking.html) 和 [Michael Ossmann](http://ossmann.blogspot.in/2010/03/16-pocket-spectrum-analyzer.html) 的工作。

固定代码系统的一个问题是它们有限的密钥空间。例如，具有 12 个二进制 dip 开关的遥控器支持 12 位的可能组合。由于它的二进制和 12 位长，那就是 2^12，也就是 4096 种可能的组合。通过一点数学计算，[Samy]表明打开一个(8-12)位的车库需要 29 分钟，假设你知道频率和波特率，这两者都很常见。如果您必须尝试几种不同的频率和波特率，那么所花费的时间是 29 分钟的倍数。如果你不多次发送代码，并消除代码之间的停顿，整个练习可以在 3 分钟内完成。

硬件中的薄弱环节是解码接收代码的移位寄存器如何工作。每个位都是按顺序载入寄存器的，随着更多位的进入并推动前一位，位会逐渐移动。这一点，再利用【Samy】基于 [De Bruijn 序列](http://en.wikipedia.org/wiki/De_Bruijn_sequence)编写的算法，整个蛮力攻击只需 8 秒多就能完成。OpenSesame 实现了这种算法，可以在最短的时间内产生每一个可能的 8-12 位重叠序列。

你可以通过在 [Github](https://github.com/samyk/opensesame) 上查看来了解代码是如何工作的。[Samy]喜欢做这样的调查工作——看看我们最近报道的他的[组合锁密码破译器](http://hackaday.com/2015/05/17/cracking-a-combo-lock-in-under-30-seconds/),恐怖的[,键盘嗅探墙疣](http://hackaday.com/2015/01/14/keystroke-sniffer-hides-as-a-wall-wart-is-scary/)和[sky jack——一种可以黑掉所有无人机的无人机](http://hackaday.com/2013/12/06/skyjack-a-drone-to-hack-all-drones/)。

[https://www.youtube.com/embed/iSSRaIU9_Vc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/iSSRaIU9_Vc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)