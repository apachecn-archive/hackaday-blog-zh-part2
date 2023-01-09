# Arduino 让 CHDK 相机遥控器成为可能

> 原文：<https://hackaday.com/2015/01/26/a-remote-for-chdk-cameras-made-possible-with-arduino/>

[AlxDroidDev]给自己做了一个漂亮的[遥控盒](http://forum.arduino.cc/index.php?topic=295377.0 "Remote control box")用于 CHDK 相机。如果你没有听说过 [CHDK](http://hackaday.com/2008/05/27/how-to-expand-your-camera-with-chdk/ "CHDK") ，这是对一些佳能相机的一个非常酷的软件修改。CHDK 为廉价相机增加了许多新功能。在这种情况下，[AlxDroidDev]使用的是一种允许通过 USB 激活相机快门的功能。CHDK 可以从 SD 卡上运行，所以不需要对相机进行永久性的修改。

[AlxDroidDev 的]设备在带有 Arduino 的 ATMega328p 上运行。它用 9V 电池供电。该电路包含一个红外接收器和一个蓝牙模块。这使得[AlxDroidDev]可以使用任何一种方法来控制他的摄像机。该设备使用标准 USB 连接器和电缆连接到相机。它包含三个 led，红色、绿色和蓝色。每一个都表示不同功能的状态。

Arduino 使用 Ken Shirrif 的红外遥控库来处理[红外遥控](http://hackaday.com/2014/09/07/infrared-controlled-light-switch/ "infrared controller lights")功能。SoftwareSerial 用于连接蓝牙模块。Arduino 代码具有用于佳能和尼康红外遥控器的内置功能。为了通过蓝牙控制相机，[AlxDroidDev]构建了一个自定义的 Android 应用程序。该应用程序不仅可以控制相机的快门，还可以控制变焦的水平。