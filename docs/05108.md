# 生日快乐，儿子。这是你自己的抓爪机

> 原文：<https://hackaday.com/2014/01/20/happy-birthday-son-heres-your-very-own-claw-machine/>

如果[威尔·巴登]参加年度最佳父亲的竞选，他将是最佳人选。他的儿子要求举办一个机器人主题的生日派对，所以[威尔]做了任何超级英雄父亲都会做的事情，[给他造了一个玩具抓爪机](http://www.youtube.com/watch?v=8CIye7Tv82c)。

[Will]从复印机上获得了许多零件:5V 和 24V 电源、限位开关、2/3 的电机和爪中的 24V 螺线管线圈。该托架来自商业印刷商。他制作了许多底座，包括装有 3 个 Pololu 步进电机的底座。

一部 [PIC16F870](http://ww1.microchip.com/downloads/en/DeviceDoc/30569b.pdf) 正在上演。[Will]使用定时器 2 对步进脉冲和 RB0 中断进行汇编编程，以在按下按钮时放下爪。如果需要的话，他还添加了一个 WDT 来摆脱代码问题。爪的螺线管由一个 [ULN2001A 达林顿阵列](http://www.st.com/st-web-ui/static/active/en/resource/technical/document/datasheet/CD00001244.pdf)驱动。[威尔]在线圈上放一个反冲二极管，这样脉冲就不会走得太远。他通过弯曲几根刹车线形成了爪形的手指。

不是你喜欢的那种爪子？看看这些不可思议的狼獾爪子！

 [https://www.youtube.com/embed/8CIye7Tv82c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8CIye7Tv82c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢，威尔]