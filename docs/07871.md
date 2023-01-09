# 插入 USB，得到一个反向外壳

> 原文：<https://hackaday.com/2014/12/21/plug-into-usb-get-a-reverse-shell/>

电脑盲目信任与其相连的 USB 设备。没有弹出窗口来确认设备是否插入，也没有验证设备是否可信。这让你可以用一个简单的 USB 微控制器做一些邪恶的事情。

我们最近已经看到了两个这样的例子:一个是 [USBdriveby](http://samy.pl/usbdriveby/) 另一个是[teensysterpreter](https://www.youtube.com/watch?v=FfRhKzbgmeU)。这两款设备都基于 [Teensy](https://www.pjrc.com/teensy/) 开发板。当连接到计算机上时，它们就像一个[人机界面设备](http://en.wikipedia.org/wiki/USB_human_interface_device_class)来模拟键盘和鼠标。

USBdriveby 以 OS X 为目标。连接后，它会将 DNS 服务器设置更改为自定义 IP，以允许受害者机器的 [DNS 欺骗](http://en.wikipedia.org/wiki/DNS_spoofing)。这可以通过 OS X 系统偏好设置实现，不需要密码，但是需要模拟击键和点击。AppleScript 用于将窗口定位在一个已知的位置，然后按钮可以被运行在 Teensy 上的代码可靠地点击。修改 DNS 后，使用 [netcat](http://en.wikipedia.org/wiki/Netcat) 打开一个反向外壳。这允许在机器上远程执行代码。

Teensyterpreter 在 Windows 机器上给出了一个反向外壳。它以管理员身份运行命令提示符，然后输入一行程序，使用 Powershell 启动反向 shell。这个过程不到一分钟就完成了，并且适用于所有比 XP 更新的 Windows 版本。

用一个 20 美元的微控制器板，你可以快速启动远程外壳，用于“支持目的”。我们希望看到这两个项目合并成一个支持两种操作系统的单一代码库。如果你能在我们的[小饰品专业版](http://store.hackaday.com/products/trinket-pro-with-black-solder-mask-and-the-hackaday-io-logo)上完成，将获得额外的积分。休息后两个项目的视频演示。

[https://www.youtube.com/embed/aSLEq7-hlmo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/aSLEq7-hlmo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/FfRhKzbgmeU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FfRhKzbgmeU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)