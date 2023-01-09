# 非数字化机械臂

> 原文：<https://hackaday.com/2014/06/03/the-un-digital-robotic-arm/>

当你想到机械臂时，你可能会想到数字控制、微控制器、电机驱动器，可能还有反馈回路。任何有幸拥有 *Armatron* 的人都知道情况并非如此，但你仍然会惊讶于[一个机械臂可以有多小](http://letsmakerobots.com/robot/project/master-slave-robotic-arm)。

[viswesh713]建造了一个伺服驱动的机械臂，没有微控制器，根据一些解释，根本没有数字控制。伺服系统由 PWM 信号控制，1 ms 脉冲使轴朝一个方向旋转，2 ms 脉冲使轴朝另一个方向旋转。有什么便宜又受欢迎的芯片可以轻松配置成定时器？是的，古老的 555。

机械臂的配置实际上更像一个主从配置的 Waldo。[viswesh]在铰链处用 pots 制造了第二个臂，pots 的电阻控制来自 556 双定时器芯片的信号输出。这是非常聪明的，至少在你意识到这是非常早期的机器人执行器是如何控制的之前是如此。尽管如此，一个简单的 555 能做什么令人印象深刻的展示。下面的视频。

[https://www.youtube.com/embed/55CRa4-ouFI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/55CRa4-ouFI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/8SmCma1kLgg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8SmCma1kLgg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

谢谢你的提示。