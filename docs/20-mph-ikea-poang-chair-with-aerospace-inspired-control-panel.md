# 20 英里/小时的宜家 pong 椅，带航天风格的控制面板

> 原文：<https://hackaday.com/2015/03/31/20-mph-ikea-poang-chair-with-aerospace-inspired-control-panel/>

工作时坐在同一把单调的椅子上，即使你幸运地使用了一把舒适的躺椅，过一会儿也会变得无聊。如果你想赢得办公室奥林匹克，你需要一些有活力的东西。[StuffAndyMakes]想造一个完全可笑的电动办公椅。经过几年的制作，他准备推出[时速 20 英里的 IKEA pong 椅子，其控制面板灵感源自航空航天](http://www.officechairiot.com/)！

他恰当地将其命名为 OfficeChairiot MkII，是一款电动[宜家 pong 舒适椅](http://www.ikea.com/us/en/catalog/categories/departments/living_room/series/07472/)。它使用现成的滑板车零件来滚动:电池、马达、链条、链轮、轮胎、车轴和轴承。OfficeChairiot MkII 基本上由三个主要部分组成——底盘、控制面板和舒适的椅子。底盘的主要部件之一是电机控制器——[Dimension Engineering Sabertooth 2×60 电机控制器](https://www.dimensionengineering.com/products/sabertooth2x60)——它也用于强壮的战斗机器人。它能承载 1000 磅的重量。并且每个马达通道可以向驱动系统提供高达 60 安培的电流。

底盘上的大脑是一个 Arduino Mega，可以通过手持遥控器控制。Mega 还接收来自各种传感器的数据，包括电机温度、电源线温度、环境空气温度、车轮转速、加速度计、座位占用和 GPS 数据。该固件旨在确保安全。手持遥控器需要每秒 ping 板载 Arduino 两次。如果由于某种原因没有收到遥控器的声音，该装置就会停止工作并关灯。

控制面板是一个疯狂的开关、按钮、显示器、导弹开关、万能钥匙开关的集合，总共有 30 多个开关和按钮。面板上的所有设备都通过第二个 Arduino Mega 控制，由定制的多路复用器板帮助连接大量设备。

这里还有一些 OfficeChairiot MkII 引以为豪的功能:

*   两个 500 瓦踏板车电机提供 1.5 马力
*   20W 立体声和 MP3 音效
*   武器声，15 种不同的屁声，汽车警报，喇叭等。
*   全 LED 照明:前灯、转向灯、88 个底盘 RGB LEDs
*   很多自制的印刷电路板
*   定制铝制车身面板(在 3D 打印汽车背后的人本地汽车公司的帮助下)

除了手工制作的木质机箱、电路板和固件，都是现成的东西。[StuffAndyMakes]计划开源原理图、C++代码和 CAD 图纸——所以在下面发表一些评论，激励他尽快这样做。我们当然希望看到更多这样的椅子被建造出来，这样办公椅比赛就会成为一项竞技运动。休息之后请看视频。

[https://www.youtube.com/embed/HZFeF6BtNf0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/HZFeF6BtNf0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)