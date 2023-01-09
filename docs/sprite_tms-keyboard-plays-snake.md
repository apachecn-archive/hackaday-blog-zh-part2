# [Sprite_TM]的键盘玩蛇

> 原文：<https://hackaday.com/2014/11/23/sprite_tms-keyboard-plays-snake/>

Hackaday 奖评委，杰出的黑客，还有一个很棒的家伙[Sprite_TM]花了很多时间在他的电脑上，这意味着他花了很多时间在键盘上打字。他最近拿起了一块在键盘世界里最流行的板，一块带有可单独寻址的发光二极管的板。他带着这块板去工作，一位同事开玩笑地说，“你已经用了这个键盘 24 小时了，它有一串发光二极管和一些箭头键。我很失望你还没有让蛇在上面跑。于是开始了将所有诺基亚手机上都有的游戏放到键盘上的探索。

有问题的键盘是 Coolermaster Quickfire Rapid-I，这是一种在市场上销售的带有 ARM Cortex CPU 的主板。拆开电路板，[Sprite]发现了一堆 MX Browns、一些 led 和一个 72MHz ARM Cortex-M3，带有 127k 闪存和 32k 内存。对于一个键盘来说，这是令人难以置信的处理能力，在找到 SWD 端口后，[Sprite]试图转储闪存。设置了安全位。然而，还有另一种方法。

Coolermaster 正在积极地改进固件，消除 bug，增加照明模式，并将所有这些更新放到他们的网站上。固件更新程序是作为美国和欧盟版本的可执行文件分发的；欧盟版还有一把钥匙。考虑到这些版本之间的唯一区别是固件本身，[Sprite]得到了这两个版本，进行了二进制比较，发现文件末尾只有一个 16k 的数据块不同。这是固件。这是异或加密，但这是显而易见的，如果你知道要寻找什么。

然而，固件并不完整；有跳转到代码[Sprite]之外的地方，一个大块看起来损坏了。对于可执行文件，还有另外一件事可以做:运行它。当执行固件更新程序时， [USBPcap](http://desowin.org/usbpcap/) 在后台运行，【精灵】可以准确读取键盘更新时发生的事情。通过一个小的可执行文件来规避更新程序的不可思议之处，[Sprite]有了键盘固件的备份。即使他用砖砌键盘，他也总能把它恢复到库存状态。是时候给 Snake 编程了。

编写新固件的第一步是找到一个有闪存和 RAM 的地方来存储新代码。这并不难；有 64k 的空闲闪存和 28K 未使用的 RAM。对 Snake 例程的调用是根据原始固件中的变量修改的。例如，如果原来的键盘有一个改变 PWM 的调用，[Sprite]可以将它改变为 Snake 例程。

Snake 很有趣，但是在一个人们可以插入键盘的设备中有一个巨大而强大的手臂，你可以用一个被黑掉的键盘做更多的事情。键盘记录器和一个 [BadUSB](https://srlabs.de/badusb/) 是极有可能的，尤其是固件可以从电脑上更新。为了应对这一点，[精灵]增加了进入闪光模式的身体条件要求。现在，按下 fn+f 组合键后固件只会更新 10 秒左右。

在键盘上玩蛇有更多的意义；Sprite 还编写了一个新的照明模式，这是一个流体模拟的东西，肯定会惹恼任何不会打字的人。你可以看下面的视频。

[https://www.youtube.com/embed/enzU9u328Fc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/enzU9u328Fc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/65c2otWBws4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/65c2otWBws4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)T2