# 把打字机变成机械键盘

> 原文：<https://hackaday.com/2015/08/27/turning-a-typewriter-into-a-mechanical-keyboard/>

你的键盘是不是太安静了？你的樱桃 MX 蓝色主板还没有让你的同事们抓狂吗？如果弯曲的弹簧键盘的机枪火力对你来说还不够，只有一个解决办法:[拉塞尔]的[打字机变成了机械键盘](http://qqrs.github.io/blog/2013/05/03/vim-on-a-mechanical-typewriter)。

将打字机改造成键盘已经有很长时间了；电传打字机是第一个计算机键盘，基本上是打字机，20 世纪 70 年代，一些 IBM 的选择键盘被改造成串行输出键盘。甚至在最近几年，在一些开关和一台 ATMega 的帮助下，打字机已经变成了键盘。[Russell]的机械键盘改进了所有这些构建，使电子界面变得非常简单，是一个任何人都可以完成的项目。

[Russell]没有在每个键下安装开关，也没有摆弄电动打字机的奇怪机械装置，而是在打字机的框架内安装了一个触敏位置传感器。当按下一个键时，它会碰到打字机框架上的横杆。通过一个 ADC 芯片和一个 Raspberry Pi，[Russell]可以确定哪个键被按下，并使用该信息向终端输出一个字符。

对于机械设备的电气接口来说，这是一个非常简单的解决方案，这个项目看起来运行得足够好。[Russell]正在使用他的 Vim 新键盘，你可以在下面的视频中看到。

[https://www.youtube.com/embed/eFBTBwdVobQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/eFBTBwdVobQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)