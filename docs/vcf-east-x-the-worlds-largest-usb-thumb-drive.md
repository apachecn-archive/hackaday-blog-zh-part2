# VCF 东 X:世界上最大的 USB 拇指驱动器

> 原文：<https://hackaday.com/2015/04/20/vcf-east-x-the-worlds-largest-usb-thumb-drive/>

上周末的复古电脑节展示了一架又一架的老式小型机，足够整个实验室使用的终端，以及足够保存 YouTube 视频的古老存储设备。这些存储设备——硬盘、磁带阅读器和 8 英寸磁盘驱动器——只连接到老式硬件，只有一个例外:[一个 DEC RL02 驱动器通过 USB](https://www.youtube.com/watch?v=T72HBhSATHY&feature=youtu.be) 连接到现代笔记本电脑。

DEC RL02 硬盘是这些旧机器中最接近现代机械硬盘的硬盘。这是一个巨大的机架单元，带有可移动的盘片，可以容纳 10 兆字节的存储空间。[Chris]发现了其中一个旧硬盘，因为他想从事 FPGA 开发，所以决定为这个巨大的旧硬盘创建一个 USB 适配器。

硬件并不太复杂，有一个微控制器和一个 FPGA，可以通过 USB 大容量存储来显示驱动器的内容。对于任何试图引导 PDP-11 或-8 系统的人来说，[Chris]可以从互联网上下载磁盘映像，将它们写入磁盘，并从小型机上加载驱动器的内容。现在，他用它和 [SimH](http://simh.trailing-edge.com/) 为一个仿真系统配置了一个物理驱动器，但是控制器并不关心磁盘组是什么格式。如果[克里斯]用一个胖文件系统格式化一个磁盘包，他将拥有世界上最大最重的 USB 拇指驱动器。

下面视频。

更新:按照承诺， [[Chris]将所有代码放入 git](https://github.com/ChrisPVille/RL02)

[https://www.youtube.com/embed/T72HBhSATHY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/T72HBhSATHY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)