# 将 Arduino 变成 USB 键盘

> 原文：<https://hackaday.com/2012/06/29/turning-an-arduino-into-a-usb-keyboard/>

新发布的 Arduino Leonardo 有几个非常有趣的功能，最明显的是由于新的 ATmega 32U4 微控制器，它可以充当 USB 键盘和鼠标。这个功能并不是 Leonoardo 独有的，正如[Michael]在他提交的一份构建中解释的那样——地位低下的 Arduino Uno 也可以通过固件更新用作 USB HID 键盘。

Arduino Uno(和 Mega)通过单独的 ATmega8U2 微控制器与您的计算机通信。只需通过 Arduino [设备固件升级](http://arduino.cc/en/Hacking/DFUProgramming8U2)上传新固件，即可轻松让您的旧 Arduino 主板获得 Teensy 或 Leonardo 等新主板的一些功能。

[Michael]完成了升级所需的步骤，并通过展示一个 Arduinofied 化的“剪切、复制和粘贴”按钮项目以及一些多媒体控件结束了他的构建。休息之后你可以在视频中查看这些构建。

如果你不喜欢模拟 USB 键盘，也可以安装 [LUFA 固件](http://www.fourwalledcubicle.com/LUFA.php)来模拟从游戏杆到 USB 音频设备的一切。非常酷，非常有用。

[https://www.youtube.com/embed/e_F9pNyTtFc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/e_F9pNyTtFc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent) [https://www.youtube.com/embed/ZKObxbaJgKI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ZKObxbaJgKI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)