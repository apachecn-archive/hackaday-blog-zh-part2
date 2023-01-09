# 球平衡机器人使用新的飞行时间传感器

> 原文：<https://hackaday.com/2015/02/14/ball-balancing-robot-uses-new-tof-sensor/>

到目前为止，您很可能已经见过甚至玩过超声波距离传感器。它们的工作原理是发出一种声音，然后听到“乒”的一声返回。然后，传感器可以通过计算两者之间的时间来判断物体离我们有多远。声波以每秒 343.2 米(768 英里/小时)的速度传播，测量声音发出，然后击中几英尺外的东西，然后返回所需的短时间可不是一件简单的事情。现在，想象一下用光来做这件事。

相比之下，光的移动速度高达每秒 299，792，458 米(约合每小时 6.71 亿英里)。你必须有一个非常快的手指放在秒表上，来测量光从几英寸远的物体反射回来所需要的时间。

[Paul Bristow]正在使用一种叫做[tera ranger One 的新型飞行时间(ToF)传感器来做这件事。](http://www.teraranger.com/product/teraranger-one-distance-sensor-for-drones-and-robotics/)该传感器与 CERN 合作开发，使用非常窄的光束(列为+/- 2 度)精确测量物体的位置，分辨率为 5 毫米，最远距离为 14 米。它拥有令人印象深刻的每秒 1000 个样本的>更新速率，并且与 UART、I2C、SPI 和 PWM 输出非常兼容。

[Paul]和他在日内瓦的[Post Tenebras Lab hacker space 的黑客伙伴们](http://www.posttenebraslab.ch/wiki/)得到了这个传感器，很快就有了一个球平衡机器人并开始运行。这个粗糙的程序没有运行一个 [PID 控制器](http://en.wikipedia.org/wiki/PID_controller)，所以休息后在视频中看到的结果并不令人印象深刻。此外，该传感器并不便宜，大约 180 美元。尽管如此，看看这些传感器将用于什么样的应用还是很有趣的。如果你有任何想法，请在下面的评论中留下。

 [https://www.youtube.com/embed/gx_XTvioWG4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gx_XTvioWG4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)