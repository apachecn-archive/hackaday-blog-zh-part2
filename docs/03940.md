# 开放式活动跟踪网络广播

> 原文：<https://hackaday.com/2013/08/28/open-activity-tracker-webcast/>

[![livedesign4](img/34f6ed60ea6fffd6841315934795cc35.png)](http://hackaday.com/?attachment_id=102053)

Upverter 团队喜欢他们的 FitBit 活动跟踪设备，但希望访问原始数据。他们决定建立自己的[开放式活动追踪器](http://upverter.com/upverter/596cf9d0bd590e03/Open-Activity-Tracker/ "Open Activity Tracker")，将数据泵入 SD 卡或蓝牙设备进行处理。

该设备使用 [MPU-9150](http://www.invensense.com/mems/gyro/mpu9150.html "MPU-9150") 运动跟踪 IC 来收集运动信息。这种芯片结合了加速度计、陀螺仪和指南针。它还进行星上处理，通过 I2C 向您的主机处理器提供有用的数据。唯一的坏消息是，这是一个 LGA 封装，手工焊接不好玩。

该设计还具有 SD 卡、蓝牙模块、压力传感器和电子墨水显示器。这些都连接到一个低功耗 ARM 微控制器。

该团队一直在网上直播他们的设计会议，今晚[Eric Evenchick](就是我)将加入他们，他们试图将所有这些元件塞进 PCB。您可以[观看东部时间晚上 8:30 开始的网络直播](http://blog.upverter.com/the-open-activity-tracker-fitbit-clone-part-4 "Open Activity Tracker Part 4")。

休息之后可以看之前的设计环节。

[https://www.youtube.com/embed/VpxpatZeiD0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/VpxpatZeiD0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/er9GnaYevyc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/er9GnaYevyc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/Sbk_1bDZFkY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Sbk_1bDZFkY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)