# Wifi 菠萝项目使用更新的硬件进行中间人攻击

> 原文：<https://hackaday.com/2013/04/29/wifi-pineapple-project-uses-updated-hardware-for-man-in-the-middle-attacks/>

我们以前见过这种小巧、廉价、功能强大的 WiFi 路由器。但这次不怀好意。【安迪】用一个 TP-Link [WR703N 搭建了一个升级的 WiFi 菠萝](http://penturalabs.wordpress.com/2013/04/25/blue-for-the-pineapple/)黑客工具。

WiFi 菠萝是 Hak5 团队几年前发明的一种设备(这里有一个展示这种设备的片段)。它使用 WiFi 路由器来响应任何 SSID 请求。基本上，如果你的电脑或智能手机保存了一个 AP SSID，并广播一个连接请求，菠萝将假装是那个设备并开始握手。这提供了在典型的中间人攻击中嗅探所有通过的数据的机会。

[安迪]正在重建设备，但价格是最低的。他花了大约 20 美元买了这个路由器，并给它加了一个 8 美元的 USB 驱动器。你唯一需要的是一个电源和隐藏硬件的方法。Hak5 版本中使用的代码可以下载，这就是他在设备上刷新 OpenWrt 后所做的工作。

[谢谢午夜]