# USB 苹果][磁盘模拟器

> 原文：<https://hackaday.com/2013/02/07/usb-apple-disk-emulator/>

在你的地下室或阁楼里放着一个旧苹果，最令人沮丧的事情之一就是缺少软件。虽然在 80 年代末的某个时候，您可能有自己的 Oregon Trail 副本，但该磁盘要么丢失，要么不起作用，并且很难将新的磁盘映像加载到 5 1/4”磁盘上。

为了给自己解决这个问题，【Eric】[想出了一个 Apple disk 模拟器](http://maclcd.blogspot.com/2013/01/karateka-and-schematic.html)。在过去的几十年里，这样的项目已经做了很多很多次，但是[Eric]有自己的想法:他不使用微控制器。相反，他使用一个简单的 USB FTDI 设备与苹果磁盘驱动器进行对话。

问题中的 FTDI 设备是一个 [UM232H 芯片](http://www.ftdichip.com/Support/Documents/DataSheets/Modules/DS_UM232H.pdf)，它采用 USB 连接，并将其转换为 SPI 总线。当然，Apple ][ disk 不支持 SPI，所以[Eric]需要用 74LS251 多路复用器和 74LS161 计数器进行一点逻辑转换。

在休息后的视频中，你可以看到[Eric]从他的新英特尔 Mac 电脑上加载苹果磁盘映像。这是一个整洁的构建，但它还没有完成:[Eric]计划添加一个带 SD 卡的微控制器，让几乎所有的苹果][游戏]都适合你的口袋。是的，[Eric]的项目与我们不久前看到的[A][pocket serial host](http://hackaday.com/2013/02/06/pocket-serial-host-acts-as-an-apple-ii-disk-drive/)非常相似，但它有望拥有更少的组件。

[https://www.youtube.com/embed/d_jsiraVC9g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/d_jsiraVC9g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)