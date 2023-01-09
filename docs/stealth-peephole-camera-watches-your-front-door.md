# 秘密窥视孔摄像机监视着你的前门

> 原文：<https://hackaday.com/2013/09/17/stealth-peephole-camera-watches-your-front-door/>

在本周的链接帖子中，我们提到了一个据称价值 4000 美元的超大功率 DSLR 窥视孔。所以当我们看到这个关于相对便宜的数字窥视孔的提示时，我们认为你们中的一些人可能对 T2 更感兴趣。

硬件相当简单；一个像样的网络摄像头，一个树莓皮，和一个供电的 USB 集线器。摄像机被剥去电路板，藏在门里。即使你从内部看到这一点，它也只是一根看起来可疑的电线，不会让大多数人认为是在使用相机。

在软件方面，[Alex]将他的 Raspberry Pi 设置为一个 24/7 网络摄像头服务器，以在线播放视频。与使用廉价的无线闭路电视摄像机不同，他的视频信号是安全的。然后他运行 [Motion，这是一个自由软件运动探测器](http://www.lavrsen.dk/foswiki/bin/view/Motion)，当有人偷偷走过时，它允许相机触发事件。它可以被设置成给你发短信、给你打电话、播放闹钟、拍照、录像……不胜枚举。如果你想复制这个系统，他的博客有完整的 DIY 指南。我们只是希望你有一个更坚固的门！

我们在 2011 年报道过一个[类似的项目，但是它使用了真正的服务器，而不是廉价的 Raspberry Pi。](http://hackaday.com/2011/04/17/webcam-turned-security-cam-with-motion-detected-email-notifications/)

【谢谢亚历克斯！]