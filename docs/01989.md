# QR 时钟对人类和计算机来说都是不可读的

> 原文：<https://hackaday.com/2012/10/29/qr-clock-is-unreadable-by-humans-and-computers-alike/>

![](img/bb49350a11118e0ae3d709af9f146bd9.png "QR")

时钟是一项完美的技术。只需几美元，你就可以买到一个数字手表和计时器，它能够在几年内保持极其准确的时间，而无需上发条或更换电池。对时钟设计的任何“改进”只会使它更难阅读，我们不时看到的 1337 个二进制时钟就利用了这一特点。[ch0f]决定是时候让位于进步的步伐，建造一个完全不可读的时钟。他发明了一种人类和手机都无法读取的二维码时钟。

硬件围绕九个 8×8 LED 矩阵面板构建，形成 24 x 24 像素的显示屏，非常适合显示 21 像素的方形 QR 码。LED 驱动器是一个标准的复用事务，但这个项目真正在固件部门大放异彩。

使用的微控制器(Ch00f)atmega 328 太小，无法存储一天中每一分钟的 1440 个二维码。不，这个项目将不得不动态生成二维码的飞行，不完全是一个简单的问题。

看了官方的二维码标准后，[Ch00f]写了[一个相当大的程序](http://ch00ftech.com/wp-content/uploads/2012/10/main1.c)，把字母数字序列转换成二维码。它每分钟都在微控制器上运行，为一天中的每一分钟生成一个新的二维码。

对于一个人来说，阅读二维码几乎是不可能的，但[Ch00f]认为他可以让他的项目变得更没用。通过以非常低的占空比复用 led，[Ch00f]使得相机不可能捕捉整个 QR 码，即使人眼仍然可以看到像素模式。一个非常无用的建筑，它真的加速了不可读时钟的游戏。

休息后的视频。

[https://www.youtube.com/embed/DLVAhHYnrbo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DLVAhHYnrbo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)