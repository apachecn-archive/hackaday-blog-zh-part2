# Game Boy 盒式仿真器使用 STM32

> 原文：<https://hackaday.com/2014/12/30/game-boy-cartridge-emulator-uses-stm32/>

游戏男孩可能是老技术，但他们仍然向现代黑客提出挑战。[Dhole] [开发了一个盒式磁带仿真器](http://dhole.github.io/post/gameboy_cartridge_emu_1/)，它使用 STMicroelectronics STM32F4 发现板来完成所有工作。到目前为止，大多数闪存卡使用可编程逻辑器件(CPLDs 或 FPGAs)来处理高速逻辑要求。【亚历克斯】[证明了微控制器](https://www.insidegadgets.com/2011/04/23/emulating-the-nintendo-logo-on-the-gameboy/)可以通过使用 Arduino 显示“任天堂”游戏男孩启动标志来模拟盒式磁带。Arduino 的速度不够快，无法处理游戏所需的高速访问。

[Dhole]通过转向基于 ARM Cortex-M4 的 168 MHz STM32F4，加快了速度。F4 的 70 个 GPIO 引脚可以通过内部外设以高达 100MHz 的速度运行，这足以处理 Game Boy 总线的 1MHz 时钟速度。逻辑电平是一个问题，因为 STM32 使用 3.3V 逻辑，而 Game Boy 是 5V 设备。谢天谢地，STM32 的输入可以耐受 5V 电压，所以一切正常。

像俄罗斯方块这样简单的游戏盒能够直接将 ROM 设备映射到游戏盒的内存空间。更复杂的游戏使用内存块控制器(MBC)芯片来映射 ROM 的各个部分并执行其他任务。有几个 MBC 芯片用于各种各样的标题，但[Dhole]可以模拟 MBC1，它与最大的代码库兼容。

[Dhole]实现的最酷的技巧之一是显示一个定制的引导标识。游戏男孩使用“任天堂”标志作为版权保护的一种方法。如果一个弹夹没有商标，游戏机就不会运行。这个标志实际上会被阅读两次——一次是检查版权信息，一次是在屏幕上显示。通过告诉仿真器在第一次读取后改变这些地址上的可用数据，可以显示任何图形。

如果你想知道卡式模拟器有什么用处(除了盗版游戏)，你应该去看看[Jeff Frohwein 的] [Gameboy 开发页面](http://www.devrs.com/gb/)！[Jeff]从早期就开始参与 Game Boy 的开发。对于 Game Boy 和各种衍生品来说，已经有几十年的演示和自制游戏了。。

[https://www.youtube.com/embed/aVxJXK9QvPk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/aVxJXK9QvPk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)