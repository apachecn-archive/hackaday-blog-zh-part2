# 一个简单的可编程 555

> 原文：<https://hackaday.com/2015/05/06/a-simple-programmable-555/>

"他可以用一个 555 定时器来代替 Arduino . ""他本可以用两个晶体管而不是 555 来做到这一点.""代替几个晶体管，他可以用蝴蝶做到这一点."这些是多年来各种 Hackaday 评论线程的引用。看起来简单是这个游戏的名字，如果你需要一个定时器芯片，8 针 DIP 怎么样？当然，这意味着以 LPC810 形式的 I2C 可编程振荡器。

[kodera2t]在多次使用 555 定时器后建立了这个电路。这是一种单芯片解决方案，采用 ARM 内核，能够产生分辨率高达 65536Hz 的方波。

[这个芯片的来源](https://github.com/kodera2t/I2C_OSC2)是大量的 C，但一旦它在 LPC810 的闪存中，这个芯片就变成了一个具有 I2C 接口的可编程振荡器。是的，这是一个单一组件的解决方案，不，这不是一个 20 美分的芯片，但尝试编程一个 555 超过 I2C。

下面的视频显示[kodera]摆弄这个 I2C 振荡器，将频率从零扫到听不见的青少年焦虑。

[https://www.youtube.com/embed/h2aHOu8kEDE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/h2aHOu8kEDE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/PkIG2ooP9_8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/PkIG2ooP9_8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)