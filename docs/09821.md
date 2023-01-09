# 黑掉一个无线网络的 SD 插槽

> 原文：<https://hackaday.com/2015/08/15/hacking-an-sd-slot-for-wifi/>

回到 20 世纪 90 年代，通过软盘移动文件被称为“运动鞋网络”虽然软盘是过去的事情，SD 卡是现代的等价物，他们仍然把自己借给运动鞋网络操作。

但是为什么呢？现在 WiFi 无处不在。如果能黑掉那些带 SD 槽的设备来用 WiFi 岂不是很棒？显然，3d 打印机[extrud3d]也有同样的想法，并找到了一种方法来重新配置东芝 flash air 卡，以将他的 3D 打印机接入网络。

该卡面向消费者，因此默认情况下，它会创建一个热点并等待连接，一个基本的网络应用程序允许你通过网络将文件来回移动到 SD 卡，然后由主机设备读取。然而，[extrud3d]展示了如何修改 SD 卡文件系统上的文件，以允许设备连接到现有的无线网络，并且还提供了一个 Python 脚本，以使文件传输更容易。

虽然这个黑客是针对 3D 打印机的，但它应该适用于大多数具有全尺寸 SD 插槽的设备(或者可以适应全尺寸卡)。因为这种攻击只不过是改变一个文本文件，所以它比我们已经讨论过的其他 SD 攻击要容易得多。在 hackaday.io 上，[克里斯·琼斯]最近对[的 FlashAir 进行了一些黑客攻击，如果你想超越文本文件黑客攻击，还有一个 shell 命令列表](https://hackaday.io/project/5558-reverse-engineering-toshiba-flashair-wifi-sd-card)。

[Kieth Wallace]为 DaVinci 打印机做了一个类似的 mod(见下面的视频),这有点复杂，因为最初的 FlashAir 卡不处理长文件名。[Kieth]不得不修改打印机的固件，尽管 FlashAir 的第 2 版可以处理长文件名，不需要太多的努力。

有一个针对 FlashAir 开发人员的[专用网站](https://flashair-developers.com/en/)，我们不得不怀疑这是否是一个通过 SD 卡插槽实现嵌入式系统网络功能的好方法(以防你厌倦了听到 ESP8266)。

[https://www.youtube.com/embed/44tMp9TTuJo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/44tMp9TTuJo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)