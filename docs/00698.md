# 给遥控直升机添加路由器和无线摄像头

> 原文：<https://hackaday.com/2012/06/11/adding-a-router-and-wireless-camera-to-a-remote-controlled-helicopter/>

![](img/5e9b2aa43b1b7460c381b439a39e537a.png "heli")

去年圣诞节，[善意的]从他的雇主那里收到了一架支持无线网络的遥控直升机。heli 是一个有趣的套件，可以用 Android 或 iDevice 控制。作为一名优秀的修理工，[bonafide]拿着螺丝刀来到他的 Wi-Fli Bladerunner 直升机上，重新设计了这个玩具，以使用现成的无线路由器。

Wi-Fli 直升机使用的协议是闭源的，但是一些人已经参与了这个酷玩具的逆向工程。除了简单地通过 WiFi 控制直升机，[bonafide]还想增加一些不受支持的功能，比如从网络摄像头发送图像。这在玩具的固件中不被支持，所以在[大胆尝试刷新新固件](http://gitorious.org/wive-rtnl-ralink-rt305x-routers-firmware#more)后，【善意】决定用 WiFi 路由器取代电子设备。

在标准配置中，直升机从基于 RT5350F 的 WiFi 模块接收命令。该模块通过串行连接与伺服系统和电机通信。[bonafide]用一个能够运行 OpenWRT 的[非常小的路由器](http://wiki.openwrt.org/toh/tp-link/tl-wr703n)替换了 WiFi 模块。新路由器很容易配置成向马达发送命令，并允许[bonafide]添加一个小的钥匙链网络摄像头，将视频流回他的桌面。

有趣的是，WiFli 直升机的制造商 Interactive Toy Concepts 将在明年秋天推出这款玩具的流媒体视频版本。WiFli 直升机的当前版本可能会在此之前进入玩具反斗城的清仓区，所以如果你想要自己的无人驾驶飞机，可能值得看看。

特别感谢[MS3FGX]发来这一篇。还有，[bonafide]网站的非 coral 缓存版本是[这里是](http://72.2.56.165:8080/)，但是尽量不要把他的服务器变成一堆熔渣。