# Illumaphone 利用光来制作音乐

> 原文：<https://hackaday.com/2014/10/05/illumaphone-uses-light-to-make-music/>

撇开特雷门琴不谈，我们还有另一种疯狂的乐器，它依靠乐手疯狂地挥动手臂来产生节拍。这是 [Illumaphone。](http://blog.bonnieeisenman.com/projects/illumaphone/)

[Bonnie Eisenman]最近参加了一个关于电子音乐的课程，在她的最终项目中，她被允许做她想做的任何事情——所以她选择创造一种定制的乐器。硬件方面相当简单，利用咖啡杯、一个 Arduino Uno、六个光敏电阻、一些鳄鱼夹和一大堆纸板——但不要让黯淡的零件清单欺骗了你，它实际上工作得很好！

每个咖啡杯都是不同的音符，进入杯子的光线量决定了它的音量和颤音。它甚至可以在首次设置时自动校准环境光线水平！Arduino 对光线水平数据进行解释，然后将其发送到待命的笔记本电脑，笔记本电脑使用一种名为 ChucK 的软件来合成音符以供输出。

[https://www.youtube.com/embed/LAt_svdEDRU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LAt_svdEDRU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/xQWdtMFZe4g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xQWdtMFZe4g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

如果这项技术对你来说太难，你可以做一个可靠的汽水罐来代替。