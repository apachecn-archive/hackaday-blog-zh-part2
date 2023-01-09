# 机器人视觉:用 FPGAs 和线激光探测障碍物

> 原文：<https://hackaday.com/2014/12/12/robot-vision-detecting-obstacles-with-fpgas-and-line-lasers/>

在路上的某个地方，你会发现你的全能自主机器人底盘将需要一些传感器反馈。否则，道路上的下一小步可能会以从咖啡桌上盲目跳下而告终。我们可能会在这个问题上扔的第一个低成本传感器将是声纳或红外测距仪，但有一个问题:这些传感器只能从正前方的精确视角提供距离数据。

请放心，[乔纳森]写信让我们知道，他有你的掩护。结合线激光器、摄像机和 FPGA，他能够探测摄像机和激光器视野内的障碍物。

如果你认为用软件写算法很难，那就等着试试硬件吧！(我们知道:组织烂透了！)[乔纳森]不知道恐惧；他在 FPGA 上直接执行梯度计算，以每秒 30 帧的速度检测相机图像中的激光。你可能会问，为什么要卷起袖子走硬件路线？如果我们在微型嵌入式机器人规模上采用基于 CPU 的方法，乔纳森估计只有每秒 10 帧。有了 FPGA，我们能够以接收图像的速度处理图像。

Jonathan 正在使用 Logi Board，这是我们过去访问过的一个成功的 Kickstarter】，他的所有代码都在 [、Githubs](https://github.com/fpga-logi/logi-projects/tree/master/logi-laser-bot "the Githubs") 上。如果你打开它，你还会发现他的许多模块都是 Wishbone 兼容的，所以只使用其中的一些部分开发你自己的项目比试图从一大堆令人毛骨悚然的逻辑中提取有用的特性要容易得多。

随着计算机视觉硬件在业余爱好者社区中保持如此低的姿态，我们很高兴听到更多关于[乔纳森的]基于 FPGA 的机器人努力。

[https://www.youtube.com/embed/SGZVa55p9Lo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SGZVa55p9Lo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)