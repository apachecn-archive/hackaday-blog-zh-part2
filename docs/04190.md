# 用树莓皮给你的车增加更多的功能

> 原文：<https://hackaday.com/2013/09/30/using-a-raspberry-pi-to-give-your-car-more-features/>

由于他的基于 Raspi 的 CarPC 项目，Andrei 正在时尚地航行，考虑到它提供的所有功能，这是一个 200 美元的便宜货。这是对三月份我们看到的[作品的更新。[Andrei]没有完全更换他汽车的主机，而是简单地将其重新放置到行李箱中，永久设置为“辅助输入”源，并连接树莓 Pi 的音频输出。Pi 和 XBMC 一起运行一个 Raspbian Wheezy 发行版，安装在中间扶手下面的存储区域。[Andrei]用一个 7 英寸的触摸屏显示器填补了旧音响留下的漏洞，它通过 HDMI 和 USB 连接到 Pi。如果您将汽车置于倒车档，Pi 会自动选择触摸屏的 AV 输入来显示汽车的备用摄像头，然后在置于驾驶档时翻转回来。](http://hackaday.com/2013/03/02/building-a-touchscreen-xbmc-setup-with-the-raspberry-pi/)

该装置还通过使用 [OpenStreetMap](http://www.openstreetmap.org/) 数据的开源 [Navit 软件](http://wiki.navit-project.org/index.php/Main_Page)提供导航。一个 [ST22 SkyTraq GPS 接收器](http://www.mr-lee-catcam.de/pe_cc_i6.htm)获取坐标并将其输入 Raspi，后者每秒更新一次屏幕上的地图。休息之后你会想看视频(音频警告:Tupac)来亲眼看看 CarPC 是如何结合在一起的，

[https://www.youtube.com/embed/0GrIyGGTRj4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0GrIyGGTRj4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)