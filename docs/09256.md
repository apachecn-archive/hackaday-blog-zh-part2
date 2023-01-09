# 移动 Kinect

> 原文：<https://hackaday.com/2015/06/11/portabilizing-the-kinect/>

早在 Kinect 第一次发布的时候，人们就意识到这款设备将会是 3D 的未来。它是增强现实，它是一种新的计算机界面，它是一种用于机器人应用的酷传感器，它是一种 3D 扫描仪。当 Kinect 的第一个开源驱动程序发布时，我们确信这是我们将真实物体的 3D 数据输入计算机的方式。

从那以后，没有发生过什么事。我们没有使用 Kinect 作为用户界面，土豆游戏玩家害怕他们会被迫购买带有新 Xbox 的 Kinect 2，你很难在机器人中找到 Kinect。3D 扫描是 Kinect 唯一没有被过度宣传的领域，即使在这个领域，它仍然是一个相对复杂的设置。

这并不意味着 Kinect 3D 扫描仪对一些人来说不是一个渴望的对象，或者不可能建立一个便携式版本。[Mario]的女朋友是一名考古学家，拥有一个 3D 扫描物体和地点的工具对她来说非常好。正因为如此，[马里奥]正在用 Raspberry Pi 2 和 Kinect 打造一款手持 3D 扫描仪[。](https://hackaday.io/project/6173-open-source-kinect-stand-alone-3d-scanner)

这不是我们第一次看到便携式 Kinect。早在 2012 年，[Kinect 在 Gumstix 板的帮助下被制成手持设备](http://hackaday.com/2012/09/16/a-portable-wifi-enabled-kinect/)。从那时起，一百万台微型 ARM 单板计算机出现了，电池组也很容易获得。迟早有人会挺身而出，而[马里奥]就是那个人。

(马里奥)面临的问题不是硬件。任何人都可以在 Gamestop 拿起一台 Kinect，Raspberry Pi 2 应该能够读取 Kinect 上的深度传感器，这些部件可以用 3D 打印部件捆绑在一起。真正的问题是软件，到目前为止[Mario]在 Pi2 上编译 Libfreenect 没有问题。该项目仍然需要很多额外的库，包括一些 OpenCV 的东西，但是到目前为止[Mario]已经一切正常。

你可以看看下面他的概念验证视频。

[https://www.youtube.com/embed/DMXKp98BY-w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DMXKp98BY-w?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)