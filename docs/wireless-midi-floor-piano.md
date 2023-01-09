# 无线 MIDI 落地钢琴！

> 原文：<https://hackaday.com/2013/11/23/wireless-midi-floor-piano/>

![123](img/f17bd95aa29456176c1be740f1473c43.png)

[李佳楠]刚刚完成他最近的一个项目的记录，[他和一个小组为](http://jiananli.wordpress.com/2013/11/20/wireless-midi-floor-piano-full-write-up/)[杜克大学的黑客马拉松制作的无线 MIDI 落地钢琴](http://hackduke.org/)！

在阅读了我们最近关于 DIY 压力板的报道后，他受到了这个项目的启发。只有 24 个小时的时间来参加黑客马拉松比赛，他们必须选择一些用便宜的材料很容易建造的东西，并能快速组装。这正是我想要的。

钢琴有 25 个铝箔压力板，其状态由 Arduino Mega 读取。然后由 XBee 无线电传输到 Arduino Uno，Arduino Uno 充当笔记本电脑的接收器来处理信号。他们甚至使用 ATtiny85 添加了一个遥控器，以允许八度音阶和乐器的变化——它还使用 XBee 与 Uno 进行通信。对于一个 24 小时的构建，质量是相当令人印象深刻的，听起来也不差——休息后听一听！

[https://www.youtube.com/embed/F218XC4n0WI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/F218XC4n0WI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

你可能还记得几个月前我们介绍过的他的另一个项目中的[李佳楠]——他的连线精美的 [试验板俄罗斯方块](http://hackaday.com/2013/09/28/breadboard-tetris-is-wire-artwork/) 游戏。