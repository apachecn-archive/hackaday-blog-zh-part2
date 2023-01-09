# 3D 打印服务器项目中的垃圾箱搜索结果

> 原文：<https://hackaday.com/2015/01/27/dumpster-dive-results-in-3d-print-server-project/>

当你很快需要一个零件时，3D 打印机非常方便。然而，如果 3D 打印机在整个打印过程中都必须连接到你的电脑上，这就非常不方便了。[Matt]购买了一台 Makerfarm i3v 打印机，并一直在使用它。他唯一不感兴趣的是让它在打印物品时占据他的电脑。然后有一天【Matt】在翻垃圾箱(别翻白眼，我们都这样)发现了一个网件 WNDR3700v1 WiFi 路由器。这个特殊的路由器有一个 USB 端口，这让[Matt]想到，“[我可以用它来运行我的打印机吗？](http://csmatt.com/notes/?p=154)

[Matt]从查看 3D 打印服务器软件 OctoPrint 开始，发现它完全是用 Python 编写的。他有一种感觉，他可以让 Python 在找到的 Netgear 路由器上运行。第一步是将 OpenWrt 安装到路由器上，并将其配置为客户机。这是直截了当的，进展顺利。路由器只有一个 USB 端口，因此需要一个集线器来连接 USB 驱动器和打印机。USB 驱动器是必要的，因为路由器本身没有足够的内存用于 OctoPrint。将 OctoPrint 安装到路由器上有点复杂，需要反复试验，但[Matt]找到了最佳方法，并在他的网站上记录下来，供有兴趣的人使用。所以现在，[Matt]可以使用他计算机的网络浏览器访问 Netgear 路由器上的 OctoPrint，开始打印，然后继续使用他的计算机，而不用担心打印失败。OctoPrint 和路由器现在单独负责控制打印机。

如果你对更多远程控制打印机的方式感兴趣，[看看这个](http://hackaday.com/2013/08/07/3d-printering-remote-control-of-3d-printers/)。