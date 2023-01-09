# 黑掉廉价的中国 PID 温度控制器

> 原文：<https://hackaday.com/2015/07/26/hacking-cheap-chinese-pid-temperature-controllers/>

黑掉了他在易贝找到的一个便宜的 PID 控制器来提高它的性能。控制器最初使用 K 型热电偶，但缺乏冷结补偿。由于热电偶仅提供测量结和冷结之间的差分测量，这意味着控制器假设冷结处于室温，在许多情况下会非常不准确。该系统还使用了一个没有品牌的中国微控制器，使得固件黑客不切实际。

[Harvs]认为，即使采用冷结补偿，K 型热电偶对他的应用也不理想，于是设计了一个替代 PCB 来连接显示器和电源。新的 PCB 基于 Cypress PsoC(因其出色的模拟功能而广受欢迎的选择)和一个 [DS18B20](http://hackaday.com/2014/02/28/smart-thermostats-for-an-old-club-house/) 温度传感器。在较低的温度范围内[Harvs]感兴趣的是，DS18B20 远比热电偶更精确且更易于使用。

虽然该项目最近没有更新，但[Harvs]正计划添加一个 ESP8266 用于远程监控。干得好！

感谢 彼得的提示。