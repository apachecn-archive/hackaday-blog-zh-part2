# 使用 HID 诡计丢弃恶意文件

> 原文：<https://hackaday.com/2015/01/27/using-hid-tricks-to-drop-malicious-files/>

[Nikhil]一直在试验与安全相关的[人机界面设备(HID)。我们](http://www.labofapenetrationtester.com/2015/01/dropping-weaponized-files-using-hid.html "Dropping malicious files via HID")[在过去已经看到](http://hackaday.com/2013/01/26/extracting-data-with-usb-hid/ "Extract data with HID")HID 是如何被廉价的设备利用的。[Nikhil]已经建立了自己的简单设备，使用 HID 技术将恶意文件投放到目标计算机上。

这个系统运行在一个小小的 3.0 版本上。Teensy 就像一个非常小的 Arduino 版本，内置了模拟人机界面设备的功能，如键盘。这意味着你可以欺骗计算机，让它相信这个小东西是一个键盘。电脑会这样对待它，青少年可以像人类打字一样在电脑上输入按键。您可以看到这可能是一个安全问题。

[Nikhil 的]设备使用一个非常简单的技巧在目标机器上安装文件。它只是打开 Powershell 并运行一行命令。通常，该命令会根据从攻击者控制的网站收到的输入创建一个文件。该脚本可能会下载特洛伊木马病毒，或者在用户桌面上创建快捷方式，从而运行恶意脚本。该设备还可以创建热键，每当用户按下该键时，该热键将运行特定的脚本。

防范这种类型的攻击是很困难的。您的主要选择是严格控制 USB 设备，但这可能很难管理，尤其是在大型组织中。在这种特定情况下，网页过滤也会有所帮助，因为攻击依赖于从网上下载文件。你最好的办法可能是训练用户不要插入他们发现的任何旧 USB 设备。不管用什么方法，重要的是要知道这些东西就在外面。