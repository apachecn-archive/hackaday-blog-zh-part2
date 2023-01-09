# 如何调暗 EL 线:电流限制振荡器！

> 原文：<https://hackaday.com/2012/10/03/how-to-dim-el-wire-current-limiting-the-oscillator/>

![](img/132526eda5387c5a32bda9400876941c.png "DreamZapper")

[Ch00f]终于在他的努力下取得了突破[调光 EL 线](http://ch00ftech.com/2012/10/02/dimming-el-wire-dreamcatcher/)。他已经做了几个月了，最后我们听说他的 [TRIAC 想法](http://ch00ftech.com/2012/08/09/method-1571-for-not-dimming-an-el-panel-triac/)已经不了了之。不要气馁，带着我们不得不钦佩的决心，他一直在努力工作[逆向工程别人的和发展自己的方法。他将所有这些知识用于帮助一位患有睡眠障碍的朋友，并制作了一个捕梦网，其脉冲频率接近普通人的呼吸频率(由苹果公司为其脉冲电源按钮灯确定)。](http://ch00ftech.com/2012/08/17/i-should-give-china-more-credit/)

本质上，整个事情可以归结为简单地使用一个晶体管来限制振荡器的电流。555 定时器用于以与苹果按钮大致相同的速率(1/5 Hz)将三角波传递到限流晶体管。[Ch00f]注意到这不是苹果使用的正弦波，但也足够好了。最后，使用十进制计数器监控 555 中三角形的数量，将超时断电内置到夜灯中。这应该可以防止 EL 线磨损得更快，尽管我们很难想到我们使用 EL 的一个项目已经持续了接近 7 年的使用寿命。

查看[Ch00f]的[页面](http://ch00ftech.com/2012/10/02/dimming-el-wire-dreamcatcher/)，他将带我们了解整个过程，或者观看他的电路在跳跃后的运行！

[https://www.youtube.com/embed/jzcYCGBHbdc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/jzcYCGBHbdc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)