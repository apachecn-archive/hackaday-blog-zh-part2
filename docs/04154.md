# 自平衡 Arduino 无需 IMU 即可实现

> 原文：<https://hackaday.com/2013/09/26/self-balancing-arduino-does-it-without-an-imu/>

这个自平衡机器人的微小尺寸使它成为一个很酷的项目。它实际上使用了小型玩具车的马达和轮子。但是，当你深入了解这种平衡行为是如何执行的，就会变得有趣得多。这种技巧的更大版本几乎都使用惯性测量单元(IMU)，通常由加速度计和陀螺仪传感器组成。这两样都没有。

机器人右侧的黑色 PCB 是一个红外反射传感器。它在地板上照射一个红外 led，并拾取反射回来的东西。[Sean]添加了这个 hack，因为他订购的陀螺仪传感器还没有到达。该板有一个微调按钮，用于调整灵敏度。你必须调整它，直到它自己站起来。休息之后自己看吧。

自平衡机器人是一个很好的自学比例-积分-微分(PID)算法的方法，这些算法在很多项目中使用。

[https://www.youtube.com/embed/iLRuapiruEw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/iLRuapiruEw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)