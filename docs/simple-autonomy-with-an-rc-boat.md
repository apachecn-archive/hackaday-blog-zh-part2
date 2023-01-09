# 遥控船的简单自主

> 原文：<https://hackaday.com/2015/06/01/simple-autonomy-with-an-rc-boat/>

[Vlad]来信告诉我们他的最新项目— [一艘在航点](http://www.instructables.com/id/Boat-Autopilot/?ALLSTEPS)之间自主导航的遥控船。建造一辆自动驾驶汽车似乎是一个非常复杂的项目，但[Vlad]的建造展示了如何在没有自动驾驶和控制系统背景的情况下制造一辆简单的路点跟踪汽车。他的设计灵感来自我们之前报道过的[侦察兵自动驾驶车](http://hackaday.com/2013/07/08/an-autonomous-boat-across-the-atlantic/)。

[Vlad]开始用 Arduino、GPS 模块和数字指南针制作原型。他写了一个快速草图，使用指南针和 GPS 读数来控制伺服系统，使其转向某个航路点。[Vlad]将他的原型带到外面，四处走动，以确保在将其放入船中之前，转向和导航工作正常。经过一点调整后，他的控制器正确驾驶，并在 GPS 位置距离目标 5 米以内时前进到下一个航路点。

接下来[弗拉德]走上了水面。他的第一次尝试是自制的汽船，看起来很棒，但不幸的是工作不太好。最后，他花 20 美元从易贝买了一艘船，并制作了一个基于 MOSFET 的电机控制器来驱动双推进器。这种设计工作得更好，经过一点 PID 调整后，船在水中的航点之间自动导航。在未来，[弗拉德]计划利用他在这个项目中学到的技能，为他父亲正在建造的[38 英尺长的双体船制造自动驾驶仪(这本身就是一个了不起的项目！).休息后观看视频，了解更多细节，并看到船在行动。](http://flipflopscat.blogspot.ca/)

[https://www.youtube.com/embed/UF1n_a_od8Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/UF1n_a_od8Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)