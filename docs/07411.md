# 随身听式人机接口设备

> 原文：<https://hackaday.com/2014/10/26/walkman-esque-human-interface-device/>

廉价的键盘从来没有额外的按钮，对于[Pengu MC]来说，这简直是不可接受的。人们没有出去买一个漂亮的键盘，而是在零件抽屉里找到了一个微控制器，并开始制作这个 [USB 多媒体按钮人机界面设备](http://pengurobotics.com/projects/media_controller)，它看起来像一个老式的随身听。

【Pengu MC】想要的功能不需要自己的驱动。该设备上的所有按钮都是 USB 键盘标准的一部分:后退、前进、播放/暂停和音量。这大大简化了软件方面，但[Pengu MC]仍然编写了自己的 HID 描述符，将所有按钮都绑定到微控制器上，并将其放在一个定制印刷的外壳中。

如果你正在寻找建立自己的类似设备，Arduino Leonardo、Micro 或 Due 都内置了这一功能，因为 USB 控制器与其他一切都集成在芯片上。一些较老的 Arduinos 也可以被编程做[同样的事情](http://hackaday.com/2012/06/29/turning-an-arduino-into-a-usb-keyboard/)！而且，使用这些项目中的任何一个，您都可以模拟任何可用的按键，而不仅仅是多媒体按钮。