# 用 FPGA 解魔方

> 原文：<https://hackaday.com/2015/06/02/solving-rubiks-cube-with-an-fpga/>

在康奈尔大学 ECE 5760 的最后一个项目中，[Alex]、[Sungjoon]和[rame ez][正在解魔方](http://people.ece.cornell.edu/land/courses/ece5760/FinalProjects/s2015/akw62_rq35_sp2283/akw62_rq35_sp2283/index.html)。他们用 FPGA 来做这件事，用自制的机器人手臂来扭转彩虹立方体，把它变成正确的位置。

首先，构建的机械部分。该团队使用了一个由三个机械臂组成的系统，分别位于立方体相对于摄像机的左、右和背面。当一个立方体被放在这个机器人的钳口中时，NTSC 摄像机数据被馈入 FPGA，在 FPGA 中，Nios II 软核处理立方体表面的实际检测、解算器算法以及向机器人手臂发送伺服命令的控制器。

用于求解立方体的算法是[CFOP](https://www.speedsolving.com/wiki/index.php/CFOP)——求解白十字、白角、中间层、顶面，最后是整个立方体。实际上，机器人最终走了 60-70 步。这不是最有效的算法；Thistethwaite 算法只需要 52 步。这种明显的低效率是有原因的 Thistlethwaite 算法需要大型查找表。

一旦立方体被扫描并计算出正确的移动，软核通过 FPGA 的 GPIO 引脚发出命令。每个立方体在扫描后不到三分钟就可以解决，但是团队遇到了扫描准确性的问题。这个问题可以通过正确的照明设置和更好的异常立方体检测以及使用 FPGAs 的伟大最终项目来解决。

下面是视频演示。

[https://www.youtube.com/embed/o-id_F1htPc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/o-id_F1htPc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)