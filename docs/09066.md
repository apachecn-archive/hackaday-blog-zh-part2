# 阀门跟踪硬件介绍

> 原文：<https://hackaday.com/2015/05/18/an-introduction-to-valves-tracking-hardware/>

[【Alan Yates】为今年的 Maker Faire 带来了 Valve 新的虚拟现实技术](http://www.hizook.com/blog/2015/05/17/valves-lighthouse-tracking-system-may-be-big-news-robotics)的演示，这是 HTC Vive 系统的基础。它非常聪明，与现有的虚拟现实耳机相比，它可能是最好的头部跟踪解决方案之一。

对于 VR 头戴设备，问题不在于将两个显示器放在用户眼前。问题是如何快速准确地确定用户在看哪里。IMU 和图像处理技术可以获得不同程度的成功，但要正确使用，它需要非常快，非常便宜。

[Alan]和[Valve]的“灯塔”跟踪装置通过在耳机上放置十几个红外光电二极管来实现这一点。在跟踪基站上，红外激光器在 X 和 Y 轴上扫描。通过在 VR 头戴式耳机上扫描这些红外激光器，可以在微控制器的几个周期内计算出耳机与基站的角度。对于一堆 1 美分的光电二极管，可以非常容易地确定相对于基站的绝对角度和方向，这在从虚拟现实到机器人的所有领域都有一些非常令人难以置信的应用。

还记得由于任天堂 Wii 使用红外信标和跟踪摄像头而出现的所有位置跟踪[黑客攻击吗？这似乎是一个进化的飞跃，但在同一领域，迫不及待地想看到人们在这项技术上黑客！](http://hackaday.com/2007/12/09/wiimote-projector-whiteboard/)