# Hackaday 复古版:AppleTalk

> 原文：<https://hackaday.com/2014/03/01/hackaday-retro-edition-appletalk/>

![retro](img/5a3a32d6c874b7ec3374f8efa87e36e3.png)

如果你通过加载我们的 Web 1.0 复古网站对经典电脑的品牌和型号进行调查，你会发现经典麦金塔电脑的数量不成比例，这些可爱的小一体机配有 9 英寸的黑色或白色屏幕。部分原因是这些盒子几乎坚不可摧的特性，部分原因是每台经典 Mac 电脑都内置了联网功能—[apple talk](http://en.wikipedia.org/wiki/AppleTalk)。

AppleTalk 的物理连接只是一个带有两个迷你 DIN 连接器(或 PhoneNet 的 RJ11 电话插孔)的小转接盒，连接到 Mac 上的一个串行端口。不过，这不仅仅是一个空调制解调器连接。一个 AppleTalk 网络可以支持多达 32 个节点、文件传输、联网打印机，以及在以后的更新中从联网驱动器引导 Apple IIGS。每当你在一个房间里有几台经典的 MAC 电脑时，AppleTalk 网络必然会在某个时候出现，特别是考虑到 800kB 磁盘驱动器对 sneakernetting 的限制以及 AppleTalk 软件随每个版本的操作系统提供的事实。

[Chris]有一台他从死亡线上带回来的旧双盘 Macintosh SE,但是他对每台电脑的互联网的现代期望意味着这台可爱的小电脑严重缺乏。是的，SCSI 到以太网适配器是存在的，但它们贵得惊人。因为有线电话，调制解调器已经过时了。他是怎么解决这个问题的？[当然是用 AppleTalk。](http://www.insentricity.com/a.cl/218/OnTheInterwebsSortOf)

在拿起一对 PhoneNet 适配器后，[Chris]将其中一个插入运行 OS 9 的 PowerPC mac。MacTCP 是用于经典 Mac 操作系统的 Apple TCP/IP 控制面板，能够将 IP 流量封装到 AppleTalk 数据包中。在将 PowerPC mac 变成路由器之后，[Chris]设法让他的一体机 SE 上网。

这种设置的唯一问题是浏览器。NCSA Mosaic 不能向代理服务器发送流量，但另一款经典的 Mac 浏览器 MacWeb 2.0c 可以。这让他能够[使用被遗忘和长期不受支持的技术来加载我们的复古网站](http://retro.hackaday.com/)。

* * *

如果你有一台旧电脑，试着用它加载我们的复古网站。拍几张照片，我们会把它放在我们的一个复古综述里