# 给 virtualbox 一个 vga

> 原文：<https://hackaday.com/2013/06/17/giving-the-virtualboy-a-vga-out/>

任天堂的 VirtualBoy——一副护目镜内的奇怪控制台，也是任天堂 3DS 的有争议的祖先——在当时是一项了不起的技术。在一个小的桌面单元中，你能够以令人印象深刻的 384 x 224 像素分辨率玩真正的 3D 视频游戏。当然，VirtualBoy 是一个彻底的失败，但这并不意味着硬件修补程序将这个美妙的系统留给了视频游戏收藏家。[furtek]一直在玩他的 VirtualBoy，[设法添加 VGA 出](http://furrtek.free.fr/?a=vbtvout)。

作为一个有两个显示器的 3D 系统，VirtualBoy 系统设计师理所当然地忽略了任何类型的视频输出。尽管如此，[furtek]想要在他的系统上显示某种视频，所以他开始用一个小 FPGA 板来产生一些 VGA 信号。

VirtualBoy 内部的两个显示器不是普通的 LCD 显示器——正如在[这个 iFixit 拆卸](http://www.ifixit.com/Teardown/Nintendo+Virtual+Boy+Teardown/3540/1)中看到的。它们实际上是两个线性 LED 阵列，产生一条 244 像素的线，反射镜在 Y 轴扫描该线。这些 led 阵列由 VirtualBoy CPU 通过一系列移位寄存器进行控制，通过仔细点击每个 LED 阵列的线路，[furtek]能够将所有图像数据复制到 FPGA 的 RAM 中。

在将 XESS XULA-200 FPGA 板塞进他的 VirtualBoy 机箱后，[furtek]为 DAC 连接了几个电阻，并在他的控制台底部安装了一个 VGA 输出端口。他第一次开机时一切正常，他开始在大屏幕电视上播放他的虚拟男孩。

因为[furtek]只读取 VirtualBoy 的一个显示器，所以当它在电视上显示时，所有的 3D 数据-以及 VirtualBoy 的主要功能-都将丢失。不过，3D 电视确实存在，我们希望看到这种电视的改进版本，可以从 VirtualBoy 的两个显示器上捕捉数据。

你可以在下面看到[furtek]的视频。

[https://www.youtube.com/embed/CCqky6sZ_R0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CCqky6sZ_R0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)