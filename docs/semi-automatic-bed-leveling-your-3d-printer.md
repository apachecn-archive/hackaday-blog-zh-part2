# 半自动调平您的 3D 打印机

> 原文：<https://hackaday.com/2015/06/29/semi-automatic-bed-leveling-your-3d-printer/>

成功 3D 打印的两个最重要的先决条件是确保床是水平的，并正确设置 Z=0 高度。获得这两个权利几乎保证了很大的粘附力，因为第一印刷层不仅在离构建平台的正确距离处，而且在部件的整个底部表面的一致距离处。

手动调平工作台很繁琐，需要用户将打印喷嘴移动到构建平台周围的不同点，调整一些螺钉，并确保喷嘴比平台高一张纸的厚度。如果您想变得复杂，有一个自动选项可以探测构建平台，并在软件中进行高度校正。探针有几种类型，两种常见的方法是部署机械开关(通常安装在伺服系统上)或构建平台下的力传感器，当喷嘴接触到构建平台时，它们会进行感应。这种方法还需要一些奇特的固件技巧才能正常工作。

[Jonas]发布了一段视频，展示了他的打印机的半自动调平功能。构建平台由弹簧保持在稍高的位置，弹簧围绕着支撑底座组件的 3 个螺钉。喷嘴直接移动到 3 个螺钉中的一个上，然后向下移动，直到它明显压在构建平台上，压缩支撑弹簧。然后在该位置拧紧拇指轮，将床锁定在适当的位置。对其他两个支撑点执行相同的过程。结果是一个完美的水平建筑表面。休息后看看视频，看看这个过程有多快！

我们已经看到了一个有点类似的概念，在床下使用了一个聪明的万向架和锁定系统。

[https://www.youtube.com/embed/8hDSFuC7HkQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8hDSFuC7HkQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)