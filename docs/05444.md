# PS4 的 USB 键盘和鼠标

> 原文：<https://hackaday.com/2014/03/02/usb-keyboard-and-mouse-for-the-ps4/>

如果你想用键盘和鼠标在 Playstation 4 上玩 BattleCallSpaceMarine 并且比其他所有在游戏机上玩的人都有不公平的优势——你通常会运气不好。索尼实施了相当多的软件来确保只有官方许可的控制器才能与控制台对话。这花了一段时间，但[Frank Zhao] [已经找出了键盘和鼠标在 PS4](http://eleccelerator.com/keyboard-and-mouse-for-playstation-4-games-second-prototype/) 上不起作用的原因，并创建了一个设备来启用这些高级输入设备。

索尼工程师决定——或者被告知 PS4 不应该连接任何旧的 USB 设备。为此，他们让控制台向 DualShock 控制器发出挑战，以确保官方控制器始终通过蓝牙连接。

[Frank]的设备通过从键盘和鼠标获取 USB 输出，进行 CRC 计算，并通过蓝牙将其发送出去，从而解决了这个问题。由于 PS4 不断发出验证程序的挑战和响应，因此需要始终将真正的 DualShock 控制器连接到设备。不过，如果你想在 PS4 上安装键盘和鼠标，这是最好的方法。

所有的源代码和布局[都在【Frank】的 github](https://github.com/frank26080115/UsbXlater) 上，你可以自由创建自己的。这还不是一个成品；[弗兰克]仍然需要重新设计电路。不过，从[对他之前在 PS4](http://hackaday.com/2013/12/13/usbxlater-for-ps4-keyboard-and-mouse-action/) 上尝试键盘和鼠标的反应来看，这可能是一款正在研发中的成功产品。