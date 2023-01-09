# 带有树莓派的全 IP 网络摄像头

> 原文：<https://hackaday.com/2014/11/03/a-full-ip-webcam-with-a-raspberry-pi/>

一台 Dropcam 大约要花 150 美元。对易贝的树莓派、摄像头传感器和闭路电视摄像头外壳进行定价，看起来可能会有更便宜的替代品来取代放在工作台上的 Dropcam，只要有人能弄清楚软件。[【Antoine】就是这么做的](http://www.sonsoftone.com/?page_id=287)，让任何树莓派都能通过网络传输 H.264 视频。

[Antoine]的软件基于基金会分发的 [raspivid 工具](http://www.raspberrypi.org/documentation/usage/camera/raspicam/raspivid.md)，但它只负责从摄像头传感器捕捉和编码 H.264 视频。为了增加 IP 摄像头支持， [Live555 RTSP 图书馆](http://www.live555.com/liveMedia/)被混合并组合在一起，通过 Raspi 的网络连接传输视频。

有了来自普通插座的摄像机圆顶外壳，[Antoine]的项目真的开始看起来专业了。规格也相当不错:它可以输出 1080 的视频流，只要对以太网线稍加修改，这个网络摄像头就有 PoE 功能。未来的更新包括基于触发器录制视频的能力，并且可能在 Pi 上配置一个 web 服务器。[Antoine]说他真的不太懂 Javascript，所以任何帮助都将不胜感激。