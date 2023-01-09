# 吓跑松鼠，用南瓜灯警告系统发微博

> 原文：<https://hackaday.com/2014/10/31/scare-off-squirrels-and-tweet-about-it-with-the-jack-o-lantern-warning-system/>

[Stephpalm]二十年来第一次雕刻了一个南瓜。不幸的是，邻居的松鼠对她的工作非常满意，狼吞虎咽地吃了起来。她发明南瓜灯的最初目标是通过互联网控制它的灯光。这些饥饿的小动物反而激发了另一个项目——南瓜灯松鼠预警系统。以前也有黑客处理过讨厌的松鼠，比如一个[陷阱](http://hackaday.com/2008/04/16/soekris-laser-guided-squirrel-trap/)和一个[自动水炮塔](http://hackaday.com/2012/03/20/birdwatching-meets-a-computer-controlled-water-cannon-awesomeness-ensues/)，但是他们没有像这个系统一样的能力发布到社交媒体上。

该系统由一个[火花核心](https://www.spark.io/)、一个[被动红外(PIR)传感器](https://www.sparkfun.com/products/8630)和一个压电蜂鸣器组成。当运动传感器被触发时，蜂鸣声响起，吓跑了任何潜伏在附近的饥饿生物。[Stephpalm]使用一个 NPN 晶体管和 1k 欧姆电阻来提供足够的电流来驱动蜂鸣器。所有这些组件都用跳线和南瓜顶部的试验板连接起来。作为对她最初想法的认可，[stephpalm]随后创建了[“南瓜手表代码”](https://gist.github.com/stephpalm/4c1a11f11547de17bb1c)，并将其加载到内核中。它每隔 45 分钟不活动，或者每当检测到讨厌的松鼠时，就会向 Twitter 账户发布预设消息。这些信息可以为任何想自己制作的人定制。

我们想知道，如果将试验板放在南瓜灯内，并在顶部挖几个孔，让 PIR 传感器的电线出来，会不会更好。这将提供一些保护元素，防止它被撞倒。我们认为这个项目可以适用于许多其他用途。休息之后，请观看系统运行的视频！

[https://www.youtube.com/embed/LrBXjMlxB38?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LrBXjMlxB38?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[通过指令]