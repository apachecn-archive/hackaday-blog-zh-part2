# 爸爸制造的火箭控制模块

> 原文：<https://hackaday.com/2014/02/17/dad-built-rocket-control-module/>

和许多父母一样，[justbennett]的孩子喜欢玩火箭和宇宙飞船指令游戏。他的孩子们的想象力分配的控制不断从这个乐高到那个香蕉再到狗的尾巴，所以[justbennett]做了他必须做的事情:为他们制作[这个爸爸制造的火箭控制模块。](http://www.instructables.com/id/Dad-Built-Rocket-Control-Module/)

该模块支持火箭和宇宙飞船管理所需的所有重要子模块。有一个发射状态指示器、一个加速度矢量谐振器(AVR)和一个 com-link。他用的大部分都是手头的零件，Arduino 的数量为零。他建造了一个美国宇航局级别的树脂玻璃外壳，以避免果汁盒事故。这两块用铝角铁连接起来，这样他就可以进行修理或修改。

模拟操纵杆是在旧货店找到的。[Justbennett]将触发器和拇指按钮连接起来作为 AVR，激活他的回收 PICAXE 08M 项目。PICAXE 感应到按钮被按下，LED 闪烁并播放升调或降调。如你所料，长按一个按钮会产生爆炸噪音。

发射状态指示器是一个电位计，连接到第二个 PICAXE 和三个依次点亮的 led。在未来，[justbennett]打算用一个微小的振动马达来增加触觉反馈。com-link 包消息传递系统是一个 Radio Shack 记录模块和两个大而诱人的按钮。控制模块配有解释控制的 Star 命令信息。