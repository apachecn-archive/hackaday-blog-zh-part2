# 伍德豪斯控制你的房子，避免危险区域

> 原文：<https://hackaday.com/2014/03/04/woodhouse-controls-your-house-avoids-danger-zone/>

![woodhouse](img/6c590a9411dec5e4e95d49eb8bc7ba8e.png)

[帕特]可能不是世界上最危险的特工，但他确实有[伍德豪斯照顾他的家](http://pathartl.me/blog/2014/03/03/woodhouse/)。在过去的几个月里，帕特一直在升级他的[声波螺丝刀家庭自动化系统](http://hackaday.com/2013/12/12/real-life-sonic-screwdriver-for-home-automation/)。醒来时房间很冷，这让他开始入侵恒温器界面。[Pat]发现他的炉子只需要一根 24v 交流电线在打供热电话时短接到公共电源上。[Pat]很幸运，因为他的恒温器是低压的。在研究恒温器黑客时，我们痛苦地发现我们的恒温器是 120VAC，所以如果你在家里尝试这个，请注意。

[Pat]把他的恒温器连接到一个由树莓皮控制的继电器上。Pi 将读取温度传感器并相应地设置继电器。这对于快速破解来说很好，但是打开一个 SSH 窗口来改变温度并不是世界上最方便的事情。输入一台旧的华硕 Transformer Prime 平板。[Pat]使用 AJAX 以及 HTML/CSS/jQuery 和 PHP 编写了一个 Android 赫萝风格的界面。OpenMic+ 不断监听语音命令，并根据需要将它们发送给[任务处理者](https://play.google.com/store/apps/details?id=net.dinglisch.android.taskerm&hl=en)任务。他把结果叫做 Woodhouse，界面非常光滑。平板电脑控制并绘制温度、[Pat 的]媒体中心和他的灯。在为那些亲密时刻做准备时，伍德豪斯甚至是 T4 的得力助手。我们迫不及待地想知道[帕特]下一步会想出什么。

[https://www.youtube.com/embed/ZZBQMjsl-aQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ZZBQMjsl-aQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/myBJAMBUPX4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/myBJAMBUPX4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)