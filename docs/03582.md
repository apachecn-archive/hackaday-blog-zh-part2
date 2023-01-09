# 纸质只读存储器

> 原文：<https://hackaday.com/2013/07/11/paper-rom/>

这种低分辨率的存储设备只能存储几个字节的数据。但这足以拼出(迈克尔·科恩的)名字。他一直在试验用纸质光盘存储数据。

当你观看下面的演示视频时，他的技术立刻变得清晰。光盘旋转多次，传感器臂读取一个磁道。这使系统有机会测量黑带，以便计算出数据时序。一旦外部磁道被读取，控制读取磁头的伺服系统将它摆动到下一个磁道，直到所有数据都被捕获。

Arduino 正在监控组成读取头的 QTR-1RC 反射传感器。它使用黑色带宽来确定单个字节的大小。有趣的是，光盘的白色部分不包含数据。数字 0 是宽度为大黑条 1/4 的黑色区域，数字 1 是宽度的一半。

[迈克尔的]设置发电机，使光盘，使他可以很容易地提高分辨率。限制因素是读取硬件能够检测到什么。

[https://www.youtube.com/embed/xtuXbxDowTg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xtuXbxDowTg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)