# 对 USB 开关的开关方式进行逆向工程

> 原文：<https://hackaday.com/2015/06/15/reverse-engineering-how-a-usb-switch-switches/>

[Daniel]发现自己需要将一个 USB 设备连接到两台 Linux 服务器。在四处寻找之后，他设法找到了一个便宜的 USB 开关。他注意到产品描述中没有提到对 Linux 的支持，但是他认为让它工作起来不会很难。

[Daniel]首先将设备插入 Windows PC 进行测试。Windows 检测到该设备并自动安装了 HID 驱动程序。下一步是在 Windows 系统上安装控制软件。这为[Daniel]提供了一个托盘图标和一个“切换”功能。单击此按钮会断开 HID 设备与 Windows PC 的连接，并在 USB 开关的另一端连接实际的 USB 设备。第二台计算机现在可以访问 HID 设备。

启动了一个叫做 SnoopyPro 的项目。该软件用于检查 USB 流量。[丹尼尔]注意到一个单一的信息重复自己，直到他按下“开关”按钮。在那时，最后的信息被发送并且 HID 设备被断开。

现在是开始破解 Linux 的时候了。[Daniel]将交换机连接到 Linux 系统，并配置 udev 规则以确保它总是显示为/dev/usbswitch。然后，他编写了一个 python 脚本，将捕获的数据写入 usbswitch 设备。就这么简单。设备按预期切换。没有 Linux 支持就这么多了！