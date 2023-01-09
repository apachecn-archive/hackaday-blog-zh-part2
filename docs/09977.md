# 令人印象深刻的 Teensy LC 装置提供的扫描电子显微镜图像和动画

> 原文：<https://hackaday.com/2015/09/05/better-image-capture-for-your-scanning-electron-microscope/>

当你有一台扫描电子显微镜时，你会想方设法推进这个令人敬畏的极限。[Ben Krasnow]正在升级他的 SEM 游戏，使用新的装备来改进图像捕捉(视频链接)并更容易地创建动画 gif 和视频。

扫描电子显微镜外壳的配色方案透露了它的 80 年代复古，当时图像捕捉技术的高度是安装在仪器 CRT 上的宝丽来相机。没有提供其他视频输出，所以[Ben]钻研蓝图并四处探索，直到他发现了高分辨率的慢扫描信号。

为了让他的 Teensy-LC 开心，他使用了几个运算放大器来调节模拟信号以获得最高分辨率，并分离出数字同步信号，分别馈入模拟和数字端口。[Ben]然后详细介绍了他是如何将视频数据编码并通过 USB 发送以进行帧捕获和 GIF 生成的。快速无抖动地读取 ADC 并平衡数据收集和传输是棘手的，但他为此建立了一个坚如磐石的系统。

[本]自己也承认，这显然是一项正在进行的工作，但它仍然非常令人兴奋。他之前制作的铁笔在黑胶唱片凹槽中的动画看起来很棒，但制作起来很费力。这里希望降低制作这些动画所需的努力会产生更多的动画。我们也希望如此！

[https://www.youtube.com/embed/ruuxn2u3yao?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ruuxn2u3yao?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)