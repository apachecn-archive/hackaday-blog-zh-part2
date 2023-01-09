# 带树莓皮的遥控野生动物摄像机

> 原文：<https://hackaday.com/2015/04/08/remote-controlled-wildlife-camera-with-raspberry-pi/>

如果你对当地的野生动物感兴趣，你可能会考虑这个[野生动物相机项目](http://anykeysolutions.org/blog/raspberrypi/pi-camera-auto-install-and-timelapse-for-android-app/ "Wildlife camera project") ( [谷歌缓存](http://webcache.googleusercontent.com/search?q=cache:QltEKJa9I7MJ:anykeysolutions.org/blog/raspberrypi/pi-camera-auto-install-and-timelapse-for-android-app/+&cd=2&hl=en&ct=clnk&gl=us))。[Arnis]一直在用他的相机拍摄狐狸和老鼠。这个构建的核心组件是一个树莓 Pi 和一个专门为 Pi 制作的红外相机模块。该系统运行在 20，000 毫安的电池上，[Arnis]声称这导致大约 18 小时的电池寿命。

[Arnis]似乎使用被动红外(PIR)传感器来检测运动。这些传感器通过检测周围红外辐射量的突然变化来工作。哺乳动物是红外辐射的良好来源，因此传感器可以很好地探测附近的动物。Pi 还连接到由继电器、电池和红外线灯组成的次级电路。当外面很黑时，[Arnis]可以启用“夜间模式”，打开红外线灯。这为在弱光条件下记录毛茸茸的动物提供了一定程度的夜视能力。

[Arnis]还在 Pi 上使用蓝牙加密狗，以便与 Android 手机通信。使用定制的 Android 应用程序，他能够连接回 Pi 并启动相机记录脚本。他还可以使用该应用程序同步 Pi 上的时间，或者从相机下载更新的图像，以确保它指向正确的方向。请务必查看下面的演示视频。

如果你喜欢这些野生动物相机，你可能想去看看一些[有类似用途的老项目](http://hackaday.com/2012/04/30/quick-and-easy-wildlife-camera/ "hacked wildlife camera")。

[https://www.youtube.com/embed/s5DENcpija4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/s5DENcpija4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

**更新:**据[报道](http://hackaday.com/2015/04/08/remote-controlled-wildlife-camera-with-raspberry-pi/comment-page-1/#comment-2518729)来自【Arnis’】页面的源代码包(名为 PiWorkingV1.7z)被病毒扫描程序标记。我们通知[Arnis]谁删除了导致误报的文件，并重新发布了该包。