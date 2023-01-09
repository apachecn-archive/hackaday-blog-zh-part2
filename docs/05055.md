# PS4 的 Arduino 库

> 原文：<https://hackaday.com/2014/01/13/an-arduino-library-for-the-ps4/>

[![PS4 Controller](img/c5ba833e7df9d4b5baf55bee081533fc.png)](http://hackaday.com/2014/01/13/an-arduino-library-for-the-ps4/ps4_controller/)

想把你的 Arduino 和 PS4 控制器连接起来吗？[Kristian]已经用对控制器的支持更新了他的 USB 主机库。该库使得从控制器读取大部分输入变得容易。目前，按钮和操纵杆可以工作，对光传感器、隆隆声和触摸板的支持正在进行中。

为了让它工作，你需要一个用于 Arduino 的 [USB 主机保护罩](http://www.circuitsathome.com/products-page/arduino-shields/usb-host-shield-2-0-for-arduino)和一个蓝牙适配器。一旦您有了硬件设置，您就可以使用库来与控制器配对。连接后，简单的函数调用将让您读取设备的状态。

虽然这确实需要一些额外的硬件来连接，但是所有的代码都是开源的。如果你想自己尝试 PS4 控制器，[Kristian]的工作可能是一个有用的起点。当然，所有的源代码都可以在 [Github](https://github.com/felis/USB_Host_Shield_2.0) 上获得，并且[示例草图](https://github.com/felis/USB_Host_Shield_2.0/blob/master/examples/Bluetooth/PS4BT/PS4BT.ino)显示了将 PS4 控制器整合到您自己的 Arduino 项目中是多么容易。