# Wii MotionPlus 陀螺仪到微芯片 PIC

> 原文：<https://hackaday.com/2015/08/29/wii-motionplus-gyro-to-microchip-pic/>

有时最普通的产品也有令人惊讶的复杂内部结构。游戏控制器里有什么？如果是 Wii 遥控器，你会发现里面有很多东西——红外传感器、蓝牙、加速度计和 EEPROM。它还有一个六针扩展端口，允许 I2C 外设连接到控制器。

[DotMusclera]想要试验陀螺仪，并决定[将 Wii motion plus](http://www.musclera.com/wii-motionplus-demonstration/)连接到微芯片 PIC。利用来自 [WiiBrew wiki](http://wiibrew.org/wiki/Wiimote/Extension_Controllers#Wii_Motion_Plus) 的信息，【DotMusclera】连接了一个 PIC18F4550、一个 LCD 和一些组件(主要是为了进行 3.3V 电平转换)，他在试验板上设置了硬件。你可能需要解决的唯一奇怪的部分是一个 Wii 分线板，它可以从试验板转换到 Wii 接口。

这个软件很容易理解，因为它是用高科技 C 语言编写的，并且受到好评。硬件缺少原理图，但从零件清单和视频中，你大概可以搞清楚。该设置运行良好，并在 LCD 屏幕上显示滚动、俯仰和偏航。

项目日志非常详细，有很多关于陀螺仪的信息，以及陀螺仪使用的通信格式。视频演示也值得一看。

Wii 遥控器被黑客攻击的时机已经成熟，我们已经看到了很多使用 T4 遥控器的 T2 项目。自然，同样的技术可以用于任何能够通过专用外设或通过位碰撞进行 I2C 的处理器。

[https://www.youtube.com/embed/MSERorNFUd8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MSERorNFUd8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)