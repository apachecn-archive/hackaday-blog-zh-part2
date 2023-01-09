# 满是灰尘的垃圾箱下变频器通过调幅收音机接收调频信号

> 原文：<https://hackaday.com/2014/10/06/dusty-junk-bin-downconverter-receives-fm-on-an-am-radio/>

这个业余无线电黑客不适合胆小的人！只有三个晶体管(和一个装满无源部件的抽屉)，[Peter Parker，vk3ye]能够[使用一个看起来很破的 AM 车载收音机来接收 2 米远的 FM 无线电信号](http://www.youtube.com/watch?v=fkzrJqK-ChQ&list=UUPhfct0hwCpv_q6_BVSFsRA) (YouTube 链接)，这是一个完全不同的波段。

这里发生了两件事。首先，一个自制的降频转换器将 147 MHz 信号下移到 AM 无线电可以处理的 1 MHz 附近。然后，调幅收音机被调谐到稍微偏离正确的频率，调频信号被检测到斜率。

下变频器由一个本地调谐振荡器和一个混频器组成。本地振荡器从一个 18 MHz 晶体产生一个大约 146 MHz 的信号，占三个晶体管中的两个。然后，使用第三晶体管将这个 146 MHz 信号和他想要收听的大约 147 MHz 信号相乘(混合)。

如果你不了解无线电理论，一个[混频器](https://en.wikipedia.org/wiki/Frequency_mixer)接收两个不同频率的信号，并产生一个输出信号，其中包含两个输入信号的各种和与差。正是这个 147 MHz–146 MHz = 1 MHz 的 FM 信号，正好在 AM 无线电波段频率范围的中间，传递到 AM 无线电。

接下来，AM 无线电[斜率检测](https://en.wikipedia.org/wiki/Slope_detector)调频(FM)信号，就像调幅(AM)信号一样。其工作原理如下:FM 无线电将音频编码为频率的变化，而 AM 无线电将音频信号编码为无线电信号的振幅或音量。斜率检测器不像调频收音机那样跟踪变化的频率，而是坚持单一频率，该频率与调频载波频率略有偏差。随着 FM 信号越来越接近或远离这个固定频率，接收到的信号变得更大或更小，FM 被检测为 AM。

5 点 23 分，[vk3ye]浏览电路图。正如他提到的，这些都是大约 50 年前的老把戏了，但很高兴看到一个垃圾箱黑客用这么少的部件工作得这么好，并在一个旧的 AM 汽车收音机上接收(非常)高频 FM。这样的电路可以成为 SDR 设置的多功能前端。它让我们想要加热烙铁。

[https://www.youtube.com/embed/fkzrJqK-ChQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fkzrJqK-ChQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

谢谢[莫里斯]的提示。