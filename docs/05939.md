# 通过 USB 使用 ThinkPad 键盘

> 原文：<https://hackaday.com/2014/04/30/using-a-thinkpad-keyboard-over-usb/>

它没有弯曲的弹簧，没有樱桃蓝色，甚至没有被遗忘的 Alps 开关，但 ThinkPads 的键盘拥有所有笔记本电脑中最好的键盘操作。他们将成为一个伟大的 USB 转换键盘，但板对板连接器很难找到，还没有人能够让键盘和跟踪点作为 USB HID 设备工作。[直到【rampadc】出现，那就是](http://www.instructables.com/id/Make-a-ThinkPad-keyboard-USB-adapter-with-Arduino/?ALLSTEPS)。

[Rampadc]的键盘适配器是为 ThinkPad T60 键盘设计的，它在联想 T60、T61、Z60、Z61、R400、R500、T400、T500 和 X41 笔记本电脑之间共享。连接器是一个非常奇怪的专有交易，可以通过通常的渠道找到，数量为 100 个，价格约为 5 美元。最重要的是，键盘没有控制器——控制器被卸载到笔记本电脑的主板上。这个键盘中唯一的电子元件只是一个矩阵。尽管如此，[rampadc]还是设法制造了一个带有十进制计数器和 SPI GPIO 扩展器的分线板。

[rampadc]制造的主板具有一个专有连接器、几个芯片和一个 Arduino Micro 插座。只需[一点点代码](https://github.com/rampadc/arduino-thinkpadkb-usb)，旧键盘就变成了现有最好的便携式键盘之一，可能比联想官方的 USB 绑定 ThinkPad 键盘还要便宜一点。

[rampadc]在 Tindie 上有一些可用的扩展板[,如果你想自己构建的话。如果你有一个这样的 T60 键盘在垃圾堆里，那才划算；不太可能出现这种情况，因为这些机器不会死。](https://www.tindie.com/products/rampadc/arduino-thinkpad-usb-keyboard-adapter/)

[https://www.youtube.com/embed/gDHS0D_EtOc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gDHS0D_EtOc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)