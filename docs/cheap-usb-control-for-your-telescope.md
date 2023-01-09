# 便宜的 USB 控制你的望远镜

> 原文：<https://hackaday.com/2015/02/20/cheap-usb-control-for-your-telescope/>

有许多复杂的系统可以自动将望远镜对准天空中的物体，但大多数对于业余天文学家来说都太贵了。[Kevin]的 Arduino ST4 接口可以让你将电脑连接到一个价格合理的电动望远镜支架上，而不用拆开它。

ST4 端口是一个非常基本的接口。底座可以移动的每个方向都有一个销，还有一个公共销。这个端口可以[添加到几乎任何机动安装](http://thx8411.over-blog.com/pages/Add_an_ST4_port_on_the_EQ4EQ5_motor_drives-3258969.html)上，只需对控制器进行一些修改。要连接 Arduino，需要使用 TLP521-4 四通道光隔离器。这使得 Arduino 和 PC 与电机电路完全隔离。但是让 Arduino 控制坐骑。

硬件到位后，[凯文]制作了一些软件，这些软件可以在谷歌代码上找到。一个简单的 Arduino 草图提供了 USB 接口，一个定制的驱动程序允许 [ASCOM 平台](http://ascom-standards.org/)控制挂载。由于许多天文学软件工具支持 ASCOM，这允许挂载由现有软件控制。

有了合适的接口，挂载就可以用来寻找物体(GOTO)并高精度地自动跟随它们(autoguiding)。休息之后你可以看到望远镜自己移动。

[https://www.youtube.com/embed/MwBNUDN8piQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MwBNUDN8piQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)