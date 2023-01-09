# 自动浇水系统使用整洁的 DIY 水阀

> 原文：<https://hackaday.com/2014/09/27/automated-watering-system-uses-neat-diy-water-valve/>

[Valentin]是一名工程系学生和业余爱好者。他计划回家度过一个为期 3 周的学期假期，当然不能让阳台上的植物自生自灭。显而易见的解决方案是制造一个[自动浇水系统](https://www.youtube.com/watch?v=6eAz3iDNdsU&list=PLLda6-GTDynjtcTCkpcso611mFPgds4f5)！

最有趣的部分是阀门。任何人都可以买到现成的电磁阀，而不是[瓦伦丁]，他自己设计的。这很简单，只要捏住供水管，就可以阻止水从 20 升的高水箱中流出。“夹紧”臂由遥控汽车伺服系统升降。当阀门处于关闭位置时，伺服机构不需要持续施加压力，伺服机构断电，阀门保持关闭。这是因为当阀门关闭时，所有的力都严格地沿径向作用在伺服驱动盘上。由于没有旋转力，驱动盘不旋转，阀门保持关闭。

伺服系统由微控制器控制。不是将伺服旋转到一定程度，而是伺服旋转直到碰到限位开关。这些限位开关告诉微控制器阀门处于开启或关闭位置。你一定在问自己‘如果限位开关失灵，而伺服系统想要继续旋转，会发生什么？’[Valentin]也想到了这一点，并让他的代码测量到达限位开关需要多长时间。如果这个时间太长，伺服系统就会断电。

下面视频。

[https://www.youtube.com/embed/6eAz3iDNdsU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/6eAz3iDNdsU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)