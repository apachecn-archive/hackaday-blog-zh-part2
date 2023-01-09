# 好吧谷歌，芝麻开门

> 原文：<https://hackaday.com/2015/02/24/ok-google-open-sesame/>

现代锁门和开门的方式多种多样。键盘、指纹扫描仪、智能卡读卡器，仅举几个例子。通常，将这些方法中的任何一种添加到旧门上都需要更换现有的锁定机构。戴上他的 Bollé太阳镜让[Dheera]想出了一个稍微新奇的主意，不用换门闩就能打开门。使用简单的现成硬件、智能手表、一些代码处理和 Google Now 应用程序，他可以在他的 Android Wear 智能手表上大喊“ [OK Google，芝麻开门](http://dheera.net/projects/sesame)”，让他的公寓门打开。

硬件，用他自己的话说，是微不足道的。一个 Arduino，一个 HC-05 蓝牙模块和一个伺服系统。伺服是附在他的门锁使用简单的硬件，看起来来自最近的五金店。代码分为两部分。HC-05 监听触发信号，并通过串行方式通知 Arduino。Arduino 反过来激活伺服系统开门。另一部分是 [Google Now 应用](https://github.com/dheera/android-sesame)。请注意，正如他明确指出的，代码是“准系统”。如果你真的想实现这种技术，明智的做法是加入身份验证，以防止所有人打开你的公寓门，偷走你珍贵的时髦太阳镜。休息后，观看他如何将所有内容整合在一起的视频。如果你感兴趣，这里有一些我们过去报道过的其他[门锁黑客](http://hackaday.com/?s=door+lock)。

[https://www.youtube.com/embed/JfZt8_a6fVY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JfZt8_a6fVY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)