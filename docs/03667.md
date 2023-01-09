# 用 Chumby 和 Bittorrent 制作 Dropbox

> 原文：<https://hackaday.com/2013/07/25/making-a-dropbox-with-a-chumby-and-bittorrent/>

![chumby](img/04d472d62aa8699751330d99ff6d93b4.png)

自从 Chumby 服务器今年早些时候下线以来，[欢]发现自己身边就有一些这种极小的、极易被黑客攻击的互联网设备。他也厌倦了他的 NAS，想要一种在所有计算机之间同步文件夹的方法。由于 BitTorrent 实验室人员的帮助，将这两种愿望结合起来，你就可以和室友一起制作个人云了。

[欢]正在使用 [BitTorrent Sync](http://labs.bittorrent.com/experiments/sync.html) 为他的 Dropbox 一样的服务器。在为 BitTorrent Sync 创建了一个 webkit 接口后，[Huan]为他的 Chumby 加载了新的固件，设置了几个要同步的文件夹，并让 Chumby 完成所有工作。

考虑到 Chumby 的无线连接和用于外部磁盘驱动器的 USB 1.1，这并不算快，但足以让您的个人项目文件夹在多台电脑之间保持同步。此外，它还非常安全，避免了云解决方案带来的大部分安全问题。