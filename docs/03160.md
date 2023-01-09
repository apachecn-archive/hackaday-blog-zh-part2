# 极其复杂的电吉他键盘

> 原文：<https://hackaday.com/2013/04/12/horribly-complicated-electric-guitar-keyboard/>

![the-email-gutar](img/8629a50e7f2038551b468f4970f6e74d.png)

冒险主义者、黑客和小胡子爱好者[大卫·尼维尔]为了将他的电吉他用作电脑键盘而聚集了太多的硬件。

因此，让我们深入研究他为这个项目建造的纸牌房子。它从吉他开始，吉他安装了一个附加的拾音器，与 Roland GR-33 合成器踏板连接。它输出一个 MIDI 信号，许多黑客会把这个信号连接到电脑上，用一个简单的脚本进行解析。但[大卫]没有，他通过 optisolator 将其连接到 Arduino。这并不太荒谬，对吧？你不认为他会解析 MIDI 信号，然后通过 Arduino 的 USB 端口把它们发送到电脑上吗？不对！他将 MIDI 信号转换成一个大的继电器板的组合，这个继电器板正在模拟一个旧的 USB 键盘的按键矩阵。但正如你在跳跃后的演示视频中看到的，它工作得很好。

如果你更喜欢打鼓，这里也有这个版本的电鼓。

[https://www.youtube.com/embed/0Er9W_oZxvY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0Er9W_oZxvY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢戴尔]