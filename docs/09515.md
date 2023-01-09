# 使用 Python 的虚拟 LCD

> 原文：<https://hackaday.com/2015/07/11/virtual-lcd-using-python/>

[Prashant Mohta]拿到了一个 16×2 的液晶显示器 Raspberry Pi，开始用 Python 写一个简单的游戏。很快，他意识到当他只想写代码时，连接 Ras-Pi 和 LCD 是很麻烦的。所以他写了一个简单的 Python 模块，在他的电脑显示器上显示 LCD。一个简单、快速、有用的方法。

[Prashant]的代码依赖于使用 [Pygame](http://www.pygame.org/wiki/about) ，这是一组为编写游戏而设计的 Python 模块。他的代码只使用了两个函数——一个定义 LCD(字符和行数),另一个通过查找数组在屏幕上绘制字符。代码不到 20 行，可以从他的 [Github repo](https://github.com/PrashantMohta/mlcd) 获得。这对那些刚开始学习 Python 的人很有用，可以帮助他们理解一些基础知识。Python 很棒，编写 Python 代码也很简单。

这可能会招致反对者的批评，所以如果你在下面评论 Python 的优点，或者不是优点，请保持你的评论文明健康。下面的视频，与这次黑客无关，【Raymond Hettinger】讲的是“是什么让 Python 这么牛逼”！

[https://www.youtube.com/embed/u1sVfGEBKWQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/u1sVfGEBKWQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)