# Java 字节码、超前的编译器和 TI-99

> 原文：<https://hackaday.com/2015/04/12/java-byte-code-ahead-of-time-compilers-and-a-ti-99/>

众所周知，Java 运行在数十亿台设备上，包括工作站、台式机、平板电脑、超级计算机和珠宝。是的，珠宝。查一下。[Michael]意识到 Java*不能在 Commodore 64s、TI-99 和一大堆其他平台上运行。[不再是了](http://www.mikekohn.net/micro/retro_console_java.php)。*

去年，[Michael]编写了 [Java Grinder](http://www.mikekohn.net/micro/java_grinder.php) ，这是一个 Java 字节码编译器，它将类编译成汇编语言，而不是 JVM 的一部分。这有效地将 Java 从即时编译语言转变为普通编译语言，如 c。他为 6502/6510、MSP430 和 Z80 编写了这种语言。然而，TI-99/4A 的 CPU 是一个奇怪的怪兽，最后[Michael]将这台 Java 研磨机转到了 TMS9900 的 CPU 上。

虽然大部分开发是用 [MESS 模拟器](http://www.mess.org/)完成的，但是【Michael】确实设法在真实的硬件上运行 Java。几年前他的朋友送了他一把 TI-99/4A，还有几发子弹。打开这些盒子，露出一个可以容纳 EEPROM 的印刷电路板。将他的 Java 字节码派生汇编写到 28c64 EEPROM 中，他就有了一个可以运行编译过的 Java 的卡带。

现在，演示非常简单，只有低分辨率的图形哔哔声和音乐，通常不是你所期望的 TI/99。这主要是因为 TI-99 的 API 非常简单。你可以在下面查看编程努力的结果。

[https://www.youtube.com/embed/Gk1-TjF576A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Gk1-TjF576A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)