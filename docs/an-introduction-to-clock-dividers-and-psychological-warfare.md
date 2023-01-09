# 时钟分频器和心理战介绍

> 原文：<https://hackaday.com/2015/04/04/an-introduction-to-clock-dividers-and-psychological-warfare/>

不久前，[nsayer]受到一篇黑客帖子的启发，开发了一种最阴险的心理战手段。当然，我说的是[【维蒂纳里勋爵】钟](http://hackaday.com/2011/10/06/vetinari-clock-will-drive-you-insane/)，一个以随机间隔滴答作响，但仍然保持准确时间的钟。他的作品“疯狂时钟”是一个用于现成时钟机芯的小型控制板，只需焊接几根电线，就可以为任何时钟添加[Vetinari]功能。

疯狂时钟是一个非常简单的设备，仅由一个 32.768 kHz 的晶体、一个微控制器和几个晶体管组成，以脉冲方式驱动时钟机构的运动。虽然心理战很棒，但最近[nsayer] [想到这个设备可以用于其他建造](http://www.geppettoelectronics.com/2015/03/repurposing-crazy-clock-as-phonograph.html)。

由于疯狂时钟的输出不一定必须与时钟运动相连，[nsayer]决定连接一个 LED，为留声机闪光灯产生 60Hz 的闪光。使用定时器预分频器和时钟分频器很容易做到这一点；原始的 32.768 kHz 信号除以 8，产生每 4.096 kHz 滴答一次的时钟。再除以 120，得到 34 2/15。是的，这些都是你在四年级学到的东西，如果你比三年级学生聪明，你最终可以将 32.768 kHz 的时钟精简为一个漂亮的圆形二进制数——这正是你计算时间所需要的。

[nsayer]贴了一个 240 fps(垂直)的视频，视频中他的疯狂时钟以 60 Hz 闪烁。你可以在下面看到。

[https://www.youtube.com/embed/4GcveFkvVWw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/4GcveFkvVWw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)