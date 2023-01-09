# 自主直升机像 Wii 遥控器一样工作

> 原文：<https://hackaday.com/2012/12/07/autonomous-helicopter-works-like-a-wii-remote/>

![autonomous-ir-helicopter](img/7e74709de5b2506e9db0f36709b84ffe.png)

[Jack Crossfire]从那些便宜的室内直升机中拿了一架，让它自动驾驶。他没有更换用于直升机的硬件，但对其进行了扩充，并接入了遥控器，制成了一个基站。

位置反馈的提供方式与 Wii 遥控器用作指点设备的方式非常相似。在游戏控制台上，电视下方有一个吧台，里面有两个红外 led。这是由 Wii 遥控器中的红外摄像头监控的，用来计算你将东西指向哪里。[杰克的]自动驾驶系统使用两个罗技网络摄像头，传感器上有红外过滤器。你可以看到他们安装在上面的切口水平酒吧。直升机本身有一个红外发光二极管添加到它总是亮着。基站通过一对伺服电机移动摄像机来跟踪信标，计算位置并在向遥控器的 PCB 发送命令时使用它。

休息后不要错过钻机的演示视频。

[https://www.youtube.com/embed/LF4bs0MUoQg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LF4bs0MUoQg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[谢谢克里斯]