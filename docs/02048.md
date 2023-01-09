# 7400 频率计数器

> 原文：<https://hackaday.com/2012/11/06/7400-frequency-counter/>

这个频率计数器是米盖尔·佩德罗索参加 7400 逻辑竞赛的作品。在看了设计之后，我们认为对于那些以前没有使用过逻辑 ic 的人来说，这是一个完美的项目。这个概念很简单，[Miguel]很好地解释了他的实现。

在它的核心，该设备只是计数一秒钟的输入信号的振荡，然后将总数锁存到 7 段显示器，然后将计数器块归零并重新开始。六个 4029 十进制计数器为该器件提供 1MHz 的范围。一组 4511 BCD 到 7 段解码器将计数转换到显示器上。4521 分频器芯片使用板载 4.194304 MHz 晶体振荡器来定时显示锁存和计数器清零。[Miguel]提到调整负载电容有点棘手。由于试验板有自己的电容问题，当移到原型板时，可能需要改变负载电容值，否则晶体不会开始振荡。你可以看到这些上限不是同一个值，但是休息后视频中的测试表明这是非常准确的。

如果你想用 HDL 来试试，这里有一个基于 FPGA 的频率计数器，你可以从中获得一些灵感。

[https://www.youtube.com/embed/DbCAFuYBilk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DbCAFuYBilk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)