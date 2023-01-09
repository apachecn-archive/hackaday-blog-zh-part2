# 在任何 Android 设备上获得外壳

> 原文：<https://hackaday.com/2013/11/17/getting-a-shell-on-any-android-device/>

如果你是一名邪恶的海关人员或其他邪恶的三字母机构人员，你可能对从人们的手机中获取数据非常感兴趣。即使屏幕被锁定，也有办法解决这个问题:只需使用 Android Debug Bridge (ADB ),这是一种在任何 Android 设备上获得外壳的便捷方法，只需一根 USB 电缆。ADB 是可以关闭的，那么如果史塔西不能通过 ADB 访问你的手机，他们该怎么办呢？[Michael Ossmann]和[Kyle Osborn] [给出了答案](http://www.youtube.com/watch?v=RHaxn1TzU3g)，这涉及到 USB 设备的一个鲜为人知的属性。

USB 迷你和微型插头有五个引脚-电源、接地、D+、D-和一个经常被忽略的 ID 引脚。通过这个 ID 引脚和地之间的特定电阻，手机内部的 USB 多路复用器可以允许任何拥有适当硬件的人访问充电器的状态，获得音频信号，摆弄你设备上的 MP3，甚至获得一个外壳。

为了测试他们的理论，[Michael]和[Kyle]在 UART 适配器上安装了一个简单的 USB 插头(见上图),其中包括一个特定值的电阻，以支持他们测试手机上的外壳。令人惊讶的是，它成功了，拥有一部安全手机的想法再也没有了。

这些人更进一步用一些三星专有的硬件，如果他们有服务手册，可以解锁任何在过去 15 年里制造的三星手机。他们正致力于制造一种设备，可以在任何手机上自动获得外壳，并且已经制造了一些相当有趣的硬件。如果你有兴趣帮助他们完成项目，[他们有一个项目网站，上面有所有的信息，可以让你快速了解这个非常巧妙的方法。](http://greatscottgadgets.com/infiltrate2013/)

[https://www.youtube.com/embed/RHaxn1TzU3g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/RHaxn1TzU3g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)