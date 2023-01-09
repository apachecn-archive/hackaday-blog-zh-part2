# [CNLohr]的显微镜载玻片 Linux AVR《我的世界》…的东西

> 原文：<https://hackaday.com/2013/02/18/cnlohrs-microscope-slide-linux-avr-minecraft-thing/>

我们一直在关注[CNLohr]的过程，即创建一个运行 Linux 的 AVR 驱动的显微镜载玻片，并将《我的世界》的 redstone 电路与真实世界的电子设备连接起来，但我们真的不知道它是如何工作的。好了，[现在有一个视频解释你想知道的关于这个令人惊讶的复杂和过度紧张的事情的一切。](https://www.youtube.com/watch?v=ENNZ5QNrHNQ)

该设备由 AVR 微控制器和以太网控制器供电，在浏览器中运行[法布里斯·贝拉]的[JSLinux](http://jslinux.org/)。[CNLohr]在 JSLinux 中添加了一些位，允许他将 JSLinux 中模拟的 x86 IO 端口映射到 AVR 的 IO 端口。这使得他只需使用浏览器就可以查询模拟和数字状态。非常酷，但[CNLohr]也可以在这台显微镜载玻片服务器上运行他的为 8 位设备优化的[《我的世界》服务器](https://github.com/cnlohr/avrcraft/blob/master/README.txt)，以在真实电子设备和 redstone 电路之间建立一座桥梁。

总结一下这里发生的事情，[Bellard]用 JavaScript 创建了一个 x86 模拟器，并把 Linux 放在上面。[CNLohr]通过连接到显微镜载玻片上电路的微控制器提供这种服务，这样他就可以在《我的世界》内闪烁 LED。基本上，这是我们见过的最漂亮的过度设计和无用的东西。

在休息后的视频中，你可以看到[CNLohr]对这台显微镜载玻片服务器的过度复杂的介绍。作为一个小小的奖励，你还可以在 00:20 在火狐浏览器的[CNLohr]最常访问/新标签中看到 Hackaday。我们很荣幸，真的。

[https://www.youtube.com/embed/ENNZ5QNrHNQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ENNZ5QNrHNQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)