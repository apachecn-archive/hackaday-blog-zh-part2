# Arduino Uno 上的 Apple ][模拟器

> 原文：<https://hackaday.com/2015/04/08/an-apple-emulator-on-an-arduino-uno/>

愚人节可能已经过去了，但我们真的必须检查一下这个黑客的日历。[Damian Peckett] [已经实现了一个 Apple ][，它的 6502 处理器，和一个盒式端口，所有这些都在一个 Arduino Uno 上。](http://dpeckett.com/turning-the-arduino-uno-into-an-apple)如果这还不够，他还使用 PS/2 键盘输入和输出模拟 VGA。[Damian]只需很少的附加组件就能做到这一切。几个电阻、一个电容和一些*非常*聪明的黑客技术都是【达米安】需要的，来让一个 Arduino Uno 相信这是一个苹果。

将所有这些工作归结为资源管理。最初的苹果[有 4KB 的内存和 8KB 的 ROM。ATmega328 只有 2KB 的 RAM，但有 32KB 的 Flash。使这种黑客工作的唯一方法是在 Flash 中保存尽可能多的仿真和其他例程，使用尽可能少的 RAM。

这次黑客攻击的核心始于苹果使用的处理器 MOS 6502。[Damian]编写了一个简单的汇编程序，将 6502 操作码和地址模式翻译成可以由 Arduino 的 ATmega328 执行的指令。为了将所有内容保存在 ROM 中并使模拟器可移植，[Damian]使用了两个大的 switch 语句。一个用于地址模式，一个 352 行的开关语句用于操作码本身。

然而，一个 CPU 本身并不是一个苹果。[达米安]仍然需要输入、输出和只读存储器，这使得苹果如此特别。通过 PS/2 键盘输入。PS/2 同步串行时钟很容易与 Arduino 接口。输出是通过[定制 VGA 实现](http://dpeckett.com/vga-on-the-arduino-with-no-external-parts)，这本身就是一个黑客。【达米安】用低级的 ATmega16u2 产生视频时序。16u2 通常用作 Arduino Uno 的 USB 接口。唯一需要的外部硬件是一个 120 欧姆的电阻。

最初的苹果有磁带和扬声器接口。这个模仿的苹果也是如此。[Woz's]原装卡带和扬声器接口精确环路，用于产生和测量频率。[Damian]在他的 6502 中接受的一个权衡是周期精度，所以他不能使用原来的例程。不过这不成问题，因为他能够编写简单的函数来替换这些例程，并删除它们来代替苹果自己的 ROM 调用。

ROM 本身被当作一个巨大的字符数组来处理。这包括系统监视器、迷你汇编程序、Sweet-16 和[沃兹]自己的整数 Basic。[Damian]通过启动他的新电脑，从磁带加载 Mandelbrot set 程序，或者在这种情况下，从他的手机上存储的音频文件，并运行它，完成了这个令人难以置信的项目。众所周知的分形在现代液晶显示器上显示得淋漓尽致，由微控制器驱动，模拟了近 40 年前的计算机。

 <http://static.dpeckett.com/apple/stream.mp4?_=1>

[http://static.dpeckett.com/apple/stream.mp4](http://static.dpeckett.com/apple/stream.mp4)

谢谢你的提示[比尔]！

苹果 II 图片由 [RAMA](https://commons.wikimedia.org/wiki/File:Apple_II_IMG_4214.jpg) ，【CC BY-SA 2.0】，通过维基共享