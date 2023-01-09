# 在 Arduino 上玩 Zork

> 原文：<https://hackaday.com/2012/04/15/playing-zork-on-the-arduino/>

[![](img/dc687f1d2c920c1626ddf6ed4ee40ab5.png "Arduino")](http://hackaday.com/wp-content/uploads/2012/04/arduino1.png)

如果你想在一个无聊的周日下午找点事做，那么掸掉你的 Arduino 和玩文字冒险游戏怎么样？[Louis]来信告诉我们他的名为 AZIP 的项目，这是一款可以让你在 Arduino 上玩 20 世纪 80 年代经典文本冒险的应用。

著名的 Infocom 文本冒险游戏，如 *Zork* 和*银河系漫游指南*(顺便说一下，据说比这本书更好)都运行在一个叫做 [ZMachine](http://www.inform-fiction.org/zmachine/interpreters.html) 的虚拟机上。我们已经看到了一些在 Arduino 上运行 ZMachine 的不成功尝试，但是这些构建通常以基于 Linux 的单板计算机结束。据我们所知，[路易斯]的建立是第一次经典文本冒险可以在 Arduino 上使用。

[Louis]基于流行的 Jzip ZMachine 进行构建。所需的硬件非常少，只需要一个带 SD 卡的 Arduino。现在 Arduino 上的闪存和 RAM 的限制意味着[Louis]需要删除游戏保存和恢复功能，但是通过一点聪明的编码和继续开发，这些功能可以恢复。确实很酷。