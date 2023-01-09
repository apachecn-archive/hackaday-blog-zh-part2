# Arduino Mega 驱动的 7x7x7 LED 立方体

> 原文：<https://hackaday.com/2013/01/31/7x7x7-led-cube-driven-by-arduino-mega/>

当然，物理构建本身看起来很棒，但最让我们印象深刻的是[迈克尔]对固件所做的。他使用 Arduino Mega 来驱动 7x7x7 立方体，并设法通过设置挤出他所谓的每秒 142 帧。我们不确定 FPS 是正确的测量方法，因为我们认为他试图描述的是多路复用率。扫描整个矩阵一次需要 144 uS。他每帧扫描七次，结果是一个无闪烁的外观，甚至对摄像机也是如此。

休息之后你可以看一段视频演示。自从[迈克尔]直接发邮件给我们，告诉我们更多关于这个版本的细节，我们也把它们贴在了文件夹下面。

如果你正在寻找一个更入门级的 Arduino LED 立方体[，这个 4x4x4 项目](http://hackaday.com/2012/01/07/minimalist-rgb-led-cube-has-a-very-short-bom/)正是你想要的。

[https://www.youtube.com/embed/CKCjsbNEUUE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CKCjsbNEUUE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

> 立方体每秒能够处理 142 帧，即每 7 毫秒处理 1 帧。在此时间段内，它在一个静止帧中循环 7 次(POV 的每个循环持续 144 微秒)。这能够补偿视频录制过程中的闪烁，允许所有摄像机无失真地录制流畅的视频。
> 
> 立方体本身由 Arduino Mega 2560 控制。对于内存中的每一帧，Arduino 会在一个编码的持续时间内读取并位移 49 字节的数据。这使得立方体可以应用于各种目的，从文本显示到效果到音乐可视化。
> 
> 这些帧是通过复杂的处理脚本生成的，允许多种操作，例如向任何方向移动(在雨效果中可以看到)，以及边缘移动(在立方体外部的滚动文本中可以看到)。这些脚本用于执行烟花计算的基础，以及 1、2 和 3 维的正弦波(见视频)。
> 
> 在这个立方体中，支撑结构由 0.9 mm 镀锌钢丝制成，通过拉伸钢丝来拉直。5 毫米蓝色 LED 相距 30 毫米，阳极连接到垂直层(下图中的白色导线)，阴极连接到水平层(下图中的绿色导线-右下方-显示为穿过 NPN 晶体管)。Arduino Mega 2560 R3 位于一个悬挂平台上，阳极由数字引脚控制，阴极由重新映射的模拟输入控制。