# 一个更好的无名氏与比格骨黑色

> 原文：<https://hackaday.com/2014/10/31/a-better-anonabox-with-the-beaglebone-black/>

几周前，Anonabox 这个设计拙劣的路由器引起了科技媒体的愤怒，它的定制固件可以保护你免受“黑客”和“合法政府”的攻击。人们发现这只是一个安装了 OpenWrt 的现成路由器，争议中的一个共同点是，“任何人都可以构建它”。这家伙没做什么新东西。

最后，一个没有想到从货架路由器上抓取另一个并放到 Kickstarter [上的可怕想法的人正在这么做](http://adammelton.com/tor_dongle.php)。[Adam]不喜欢 Anonabox 的缺点，并查看了保持在线匿名的最佳实践。作为回应，他设计了一个 Tor dongle，并配有一个 Beaglebone Black。

[Andy]没有像 Anonabox 和许多其他项目那样使用无线技术，而是将 Beaglebone 用作加密狗/以太网适配器，所有数据都通过 USB 端口传输到计算机。不会，它不会保护您的整个网络；只有一个设备，而且只有在插上电源时。

安装过程非常简单，只需安装所有相关软件，卸载所有 cruft，然后配置一个浏览器。[Adam]通过他的 Tor ified 以太网适配器，在只使用 40% BBB CPU 的情况下，能够获得 7Mb/秒的速度下降和 250 kb/秒的速度上升。