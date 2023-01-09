# 结合 3D 打印和机器人技术的自动化家庭制造

> 原文：<https://hackaday.com/2014/06/01/automated-home-manufacturing-combining-3d-printing-with-robotics/>

[Florian]一直在努力工作，为他的 3D 打印机创建这个自动设置来排队作业，以便在他不在的时候运行它。虽然还没有完全完成，但是概念已经有了，他已经开始做一些测试了！

他使用的是 [uArm](http://www.ufactory.cc/) ，这是今年早些时候非常成功的[kickstarter](https://www.kickstarter.com/projects/ufactory/uarm-put-a-miniature-industrial-robot-arm-on-your)——这是一款兼容 Arduino 的微控制器驱动的 4 轴平行机械机械臂，基于工业 [ABB PalletPack 机器人。](http://new.abb.com/products/robotics/industrial-robots/irb-460)

他一拿到所有的部件，就设置了一个快速测试来替换使用 uArm 的构建平台。

[https://www.youtube.com/embed/IO4n2VAmRII?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/IO4n2VAmRII?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

我们现在看到的唯一问题是 3D 打印可能会在中间！更换床很好，但也需要安全。通常[Florian]使用活页夹，但对于机器人来说，这些太挑剔了，所以他正在研究一种磁性夹紧系统，这种系统既足够强大，可以将床固定在适当的位置……又足够容易让 uArm 自己移除:

[https://www.youtube.com/embed/xWjg7n46620?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xWjg7n46620?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

我们非常兴奋地看到这方面的持续进展。将它与一台带有网络摄像头和某种远程桌面的专用计算机(免费版的 [TeamViewer](http://www.teamviewer.com/en/download/windows.aspx) 工作得相当好)相结合，您就可以在旅途中完全控制您的设置了！