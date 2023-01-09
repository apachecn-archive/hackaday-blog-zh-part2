# 小心艺术家，机器人接下来会抢走你的工作

> 原文：<https://hackaday.com/2014/09/16/watch-out-artists-robots-take-your-job-next/>

在克洛德·莫内，出现了一种新的行为，一种能够创造一些非常酷的艺术的机器人。

我们以前见过机器人艺术家，但他们中的大多数要么是基于笛卡尔坐标的，要么是悬挂的 T2 绘图机器人。这是一个羽翼丰满的机器人手臂，挥舞着锋利的笔尖，用点画图，给它的作品一种印象主义的感觉。

实际的机械臂是库存的 Interbotix。幻影多媒体公司的人写了一些定制的软件，可以把一个图形分解成一个 1 比特的表示。然后，代码随机遍历位图，挑选点在介质上绘制。这个项目的难点在于如何将 2D 的图像转换成 3D 机械臂的运动。因为手臂有几个关节，所以对于将标记移动到任何给定点的手臂位置有多个数学解。该团队最终编写了一个算法来确定从一点移动到另一点的最有效方式。即便如此，每幅画都要花几个小时。

好像这还不够，软件被重新设计来探测位置。不是自动地将臂移动到预定点，而是手动地将臂移动到一个位置，并且从伺服编码器取回的数据用于确定臂末端的探针的位置。以这种方式获得的每个点然后可以被组合以生成 3D 模型。

[https://www.youtube.com/embed/2QPjh5Q1XOs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/2QPjh5Q1XOs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

谢谢你的提示[亚当]