# 两轮车是陀螺仪稳定的

> 原文：<https://hackaday.com/2014/05/08/two-wheeler-is-gyroscope-stabilized/>

[Jim]喜欢陀螺仪——不是那些新奇的 MEMS 设备，而是老式的机械陀螺仪。他的痴迷促使他建造了这个[陀螺稳定的两轮车](http://letsmakerobots.com/content/gyro-stabilized-two-wheeler-v5-steering)。我们喜欢看简单的基本材料和手工工具组合在一起，用大量的热熔胶将一切固定到位。这似乎也是[吉姆]的哲学。

这实际上是[吉姆的]设计的第五个化身。一路上，他学到了一些关于机械陀螺设计的重要秘密，比如平衡电机和陀螺组件，使其有点头重脚轻。[Jim 的]陀螺仪是一叠 CD，直接安装在一个有刷 speed400 R/C 飞机马达的轴上。马达以极快的速度旋转光盘——毫不夸张地说。[Jim]提到他们在他早期的一些实验中爆炸过。

陀螺仪可以在前后方向自由移动。左右平衡倾斜取决于车轮本身。轮子是模型飞机轮子，有一个弯曲的胎面。不要在[吉姆的]实验室里用扁平的乐高轮子作弊！电位计测量陀螺仪的倾斜角。来自电位计的电压被馈入 Arduino Uno，它通过移动安装在伺服系统上的配重来闭合回路。

车辆由常规遥控飞机无线电控制。一个伺服转向前轮，而另一个 DC 电机驱动后轮。[吉姆]的作品不仅能够自行平衡，甚至还能在走廊里掉头。

[https://www.youtube.com/embed/arcIC_EKOcE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/arcIC_EKOcE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/NsBnBMIeXeo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NsBnBMIeXeo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)