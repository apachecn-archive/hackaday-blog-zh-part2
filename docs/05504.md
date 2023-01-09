# 遥控快门让你从远处成为一个潮人

> 原文：<https://hackaday.com/2014/03/11/remote-shutter-release-lets-you-be-a-hipster-from-a-distance/>

![camera shutter](img/461c9d61194f638c2e51c66184f0bc3b.png)

所以，你用你古老的中画幅胶片相机拍摄高分辨率照片——但是你不能在相机前。好吧，如果你是[curlyfry562]你可以自己制作[遥控机械快门！](http://www.instructables.com/id/Remote-Mechanical-Shutter-Release)

由于胶片相机的年代，真的不多(或者说……有？)解决这个问题的现成方案。特别是没有与项目目标列表[curlyfry562]一起想出:

*   它必须由远程 TTL 信号触发
*   无线范围必须至少为 100 英尺
*   它必须可靠——中画幅胶片很贵！
*   它需要易于安装和拆卸

目标明确后，他开始工作。他使用的 2.4GHz xBee 调制解调器有一个 DIO 引脚——如果你连接两个用于 DIO 线路传输，那么它们就像彼此的克隆——改变一个的状态，另一个就会跟随。利用这一点，他将输出连接到一个微控制器，然后驱动伺服系统按下机械快门。这其实非常简单。

如果你不需要那么大的范围——看看这个由无线门铃制成的遥控快门按钮！

【谢谢大牛！]