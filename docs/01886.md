# 用意念控制机器人

> 原文：<https://hackaday.com/2012/10/15/controlling-a-robot-with-your-mind/>

![](img/b2e5840851bf10d7054bf177b6fec8ca.png "mindwave")

对于[Ern]的孟小组项目，他的小组必须开发一个能够实现某些最终目标的机器人平台。因为创新是分数的很大一部分，[Ern]说服他的团队成员用大脑控制的界面工作，并建立一个[大脑控制的机器人平台](http://ernarrowsmith.wordpress.com/2012/10/02/a-basic-neurorobotics-platform-using-the-neurosky-mindwave/)。

为了不容易制造，[Ern]和他的团队选择了一个能够在教室里移动的 Lynxmotion 三轨道机器人，同时接收计算机的命令。该建筑的精神控制部分来自 [NeuroSky MindWave Mobile](http://store.neurosky.com/products/mindwave-mobile) ，这是一种廉价且相当开放的脑电图系统，可以读取用户大脑产生的α、β和δ波，并将数据发送到计算机进行处理。

经过一段时间的测试，包括 Arduino 在 MindWave 的“注意力”值超过 60%时推动机器人前进，[Ern]和他的团队寻找一种实现多方向控制的方法。

为了让机器人除了向前移动之外还能向左、向右和向后移动，该团队研究了 MindWave 的“眨眼检测”能力，以循环执行几个命令。这项技术被证明过于敏感——意识波的眨眼检测简直太好了。为了解决这个问题，研究小组使用了接收到的脑电图信号的信号强度。理论是当用户眨眼时，脑电图触点会轻微移动，降低硬件接收的信号。

该团队最终让一个合理的精神控制机器人启动并工作，正如休息后的视频所示。看看每次眨眼是如何让[Ern]和他的同事在驾驶模式中循环的。用你的思想控制某些东西真是太棒了。

[https://www.youtube.com/embed/0-YuF9z5-uI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/0-YuF9z5-uI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)