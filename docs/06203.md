# Propeddle，软件定义 6502

> 原文：<https://hackaday.com/2014/06/01/propeddle-the-software-defined-6502/>

当谈到建造逆向计算机时，有两种想法。首先是仿真，它允许更好的兼容性和易用性，并且更容易找到部件。第二种需要真正的老式硬件，拥有老式芯片中的所有缺陷和特性。调和这两种想法是困难的，但是软件定义的 Propeddle 设法做到了这一点，同时使用了一个真正的 6502 CPU。

这里的技巧是使用 Parallax Propeller，以极其巧妙的技术将 ROM 加载到 RAM，使用 Reset 和 NMI 引脚，生成 6502 所需的时钟和其他信号，并托管键盘、串行和视频 I/O。已经[Jac]拥有作为 Apple 1 仿真器运行的 propedle(如下视频)，这使得用 BASIC 或 assembly 编写 propedle 程序成为可能。

这是一个伟大的设计，它允许模拟许多具有真正 CPU 的经典 6502 计算机，同时消除了昂贵的 ACIAs 和视频生成硬件的不足。令人敬畏的工作，我们不能等待下一个版本[将致力于【比尔门施】](http://propeddle.com/)。

[https://www.youtube.com/embed/8BCoQepmyYU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8BCoQepmyYU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)