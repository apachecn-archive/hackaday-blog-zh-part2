# 将 Wii U 控制器与一切一起使用

> 原文：<https://hackaday.com/2013/12/30/using-the-wii-u-controller-with-everything/>

距离 Wii U 和令人印象深刻的 Wii U 控制器一起发布才一年多一点。凭借 D-pad、模拟杆、加速度计、陀螺仪、磁力计、摄像头和 6.2 英寸触摸屏，这款控制器已经成熟，可以用于从 FPV 四轴飞行器和机器人到我们甚至想不到的东西的一百万个项目。在今年的混沌通信大会上，[booto]、[delroth]和[shuffle2]展示了他们如何破解了 Wii U 控制器的加密，允许 Wii U 控制器“仿真”，并为我们提供了关于整个事情如何工作的完整文档。

这些人开始了他们的逆向工程之旅，他们扔掉了控制器板上所有的闪存芯片。在这些二进制 blobs 中，他们发现任天堂使用了一种真正巧妙的方法来混淆用于连接控制器和 Wii 的 WiFi 键:向左旋转三度。公平地说，对任天堂的工程师来说，在有人发现之前，它是安全的。

然而，通过 WiFi 将控制器连接到电脑只是成功的一半。Wii U 发布会的最初信息表明，任天堂将 Miracast 用于控制器和控制台之间的所有 I/O。事实并非如此。相反，视频、音频、摄像头和按钮输入都是非标准但非常简单的协议。最难侵入的是触摸屏的视频显示，但这些人发现它几乎是 H.264。在解决了一些任天堂的古怪问题后，它可以在控制器上显示视频。

这些家伙已经把[一个小型的、非常 alpha 化的库](https://docs.google.com/presentation/d/126fk9mO5jROMfuw-2ASDv7-YH_A0LZO0Phxedh9deiE/edit?pli=1#slide=id.g261110b57_8121)放在了一起，里面有所有的演示、文档和逆向工程信息。有一个很大的愿望清单，这个图书馆应该包括什么，但现在信息是公开的，可能是时候拿起一个 Wii U。

下面是演讲的视频，[这是演示幻灯片](https://docs.google.com/presentation/d/126fk9mO5jROMfuw-2ASDv7-YH_A0LZO0Phxedh9deiE/edit?pli=1#slide=id.g261110b57_70)，还有[一个在 PC 上模拟 Wii U 游戏手柄的演示](http://www.youtube.com/watch?v=Yt2-IRiWd40)。

[https://www.youtube.com/embed/m8YgVVtNRjg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/m8YgVVtNRjg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)