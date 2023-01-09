# 一切使用 XBox One 和 PS4 控制器

> 原文：<https://hackaday.com/2013/12/07/using-xbox-one-and-ps4-controllers-with-everything/>

上一代游戏机的控制器很好地服务了他们的目的。当我们想用 I2C 巴士做实验时，他们就在我们身边；当我们想用闲置的零件造一架四轴飞行器时，他们就站在我们旁边。新一代游戏机已经在我们面前，随之而来的还有新的控制器。Arduino 库尚未编写的控制器。恐怖。

在这些库开发出来之前，[还有 ChronusMAX](http://cronusmax.com/) ，一个 USB 加密狗，允许你在 PS4 上使用 XBox One 控制器，在 XBox 上使用 PS4 控制器，在两个系统上使用鼠标和键盘，在 PC 上使用这两种类型的控制器。

ChronusMAX [的工作人员发布了一个视频](http://www.youtube.com/watch?v=qA4gu-iuIVw)演示 XBox One 控制器在 360、PS3 和 PC 上的工作，[发布了另一个视频](http://www.youtube.com/watch?v=RkbjUj5nN6g)演示 PS4 控制器的工作情况。就我们从 PC 演示中看到的来说，这些控制器上的一切都可以读取，甚至可以读取 DualShock 4 上的加速度计数据。

虽然这是一个商业产品，但我们很惊讶到现在还没有看到一个更开放的版本。从外观上看，它是一个非常小的设备，有两个 USB 端口和一个固件上传工具。带有两个本机 USB 端口的微控制器通常封装在大型封装中，因此该器件中可能有一些非常聪明的工程设计。如果有人拆了这些东西，请告诉我们。

谢谢[乔希]送来这个。