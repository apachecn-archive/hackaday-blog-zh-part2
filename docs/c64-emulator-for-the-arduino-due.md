# Arduino 的 C64 仿真器到期

> 原文：<https://hackaday.com/2014/07/06/c64-emulator-for-the-arduino-due/>

![c64](img/4031c66c065cedab048c221148a06f82.png)

大约一年前，[miker00lz] [在 Arduino 论坛](http://forum.arduino.cc/index.php?PHPSESSID=son476sue1n5pj4sdj15v57hf2&topic=193216.0)上发了一个帖子，告诉大家他为 Arduino Uno 编写的 6502 仿真器和 BASIC 解释器。Uno 内部的芯片无论如何都不是一个强大的处理器，只有 2KB 的内存，远远不如 70 年代的任何一台电脑。然而，Arduino 可以在许多不同的芯片上工作，几个月后，[Jan]将一个 Arduino Due[变成了一个 Commodore 64 模拟器](http://forum.arduino.cc/index.php?PHPSESSID=cc7tt1eirmqh1bpjg8gbvreet5&topic=193216.msg1791372#msg1791372)。

[Jan]的代码不限于 DUE，可以用在任何有足够内存的芯片上。如果你觉得有趣，你可以连接一个 TFT 显示器来获得 PETSCII 图形的所有优点，同时运行一个比非常精简的 EHBASIC 更快的 BASIC。

因为仿真器使用软件与外界交流，所以应该可以使用这个项目与 Commodore 机器中的较冷芯片接口——例如 sid，但也可以作为老式以太网的盒式端口。它甚至不局限于 Commodore 机器:在 Atari 8 位微处理器中发现的小芯片在 chiptune 和 demoscene 中严重利用不足，让现代硬件与这些芯片一起玩不会有丝毫损害。

[https://www.youtube.com/embed/NvQe6eg5_hQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NvQe6eg5_hQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)