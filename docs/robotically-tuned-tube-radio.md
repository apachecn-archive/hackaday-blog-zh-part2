# 自动调谐电子管收音机

> 原文：<https://hackaday.com/2014/12/27/robotically-tuned-tube-radio/>

被[布雷克]称为“[”机器人无线电](http://forums.hackaday.com/viewtopic.php?f=3&t=3892)”的这个叮当作响的-&-咯咯作响的项目融合了三代黑客最喜欢的技术:机器人、真空管和微控制器。在人类输入想要的无线电频率后，机器在频谱中凿出一条路，尽最大努力停留在目标上。

这座建筑开始时是一台破烂的旧电子管收音机，是从一个棚子里拖出来的。案件恢复，然后黑客攻击开始。PIC 16F628A 插在人和无线电之间，保持两个方向的监视。一方面，收音机的储能电路被监控，以查看收音机当前播放的频率。另一方面，人类的输入设定了期望的频率。如果两者不匹配，PIC 告诉步进电机开始转动一对齿轮，直到它们匹配。

另一个有趣的特点是，当电子管和其他电子设备升温并改变它们的值时，匹配电路会使它们保持一致。[Brek]在视频中展示了这一点，故意破坏齿轮，并看到机器人将它们调整回它们应该在的地方。

事后，机器人无线电补充了一个模块，增加了 100khz 的信号，以便可以接收附近机场的信息。

[Brek]用一些铜框架和其他零件将整个机器装饰起来，类似于我们上个月介绍的他的壮观的[原子钟](http://hackaday.com/2014/11/27/jaw-dropping-atomic-clock-build/)建造。

休息后看收音机调音的视频。

(注:没错，前几秒缺音频，不只是你。等等吧。)

(注 2:没错，除了最后一个，线程里所有的进度 vid 都被删了，不只是你。)

[https://www.youtube.com/embed/LfJNT3XWDRg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LfJNT3XWDRg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)