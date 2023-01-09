# ATtiny10 上的 USB

> 原文：<https://hackaday.com/2014/03/20/usb-on-the-attiny10/>

就物理尺寸而言，Atmel 的 ATtiny10 是他们最小的微控制器——它是 SOT-23-6 封装，大约与表面贴装晶体管相同。这里面的硬件极其简单；三条 I/O 线、1kB 闪存、32 个*字节*的 RAM，以及一个 16 个寄存器而不是 32 个寄存器的精简 AVR 内核。有了这样一个最小的功能集，你可能会认为这款微处理器唯一擅长的就是闪烁 LED。你可能是对的，但是[cpldcpu] [可以通过“tiny10 over USB”使 LED 闪烁。](http://cpldcpu.wordpress.com/2014/03/19/%C2%B5-wire-usb-on-an-attiny-10/)

V-USB 接口在其最简单的实现中通常需要大约 1.5kB 的闪存，并使用 50 字节的 RAM。这对于 tiny10 来说是不行的，尽管[cpldcpu]正在开发一种更小的、无中断的 V-USB，但仍然有一些障碍需要克服。

将代码放在 tiny10 上的最大问题是其精简的 AVR 内核——在“大”32 寄存器内核上，直接内存访问是两个字。在 10 年，只有一个词。AVR-GCC 不知道这一点，Atmel 似乎也没人在意。[cpldcpu]使用 defines 解决了这个问题，并通过完全删除 V-USB 并将其放入主循环中进一步减少了代码大小。

不算多，但是现在[cpldcpu]可以用' tiny10 over USB '来闪烁 LED。如果你想知道，这个项目使用了 96.4%的 Flash 和 93.8%的 SRAM。