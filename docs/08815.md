# Energia 多任务处理在 MSP432 上使用 RTOS

> 原文：<https://hackaday.com/2015/04/17/energia-multitasking-uses-rtos-on-msp432/>

随着硬件变得越来越强大，我们一直想知道 Arduino 世界将走向何方。如果 IDE 跟不上，还有什么意义呢？现在我们对这个问题至少有了一个答案。Energia 是德州仪器基于主板的类似 Arduino 的框架。他们刚刚推出了 Energia 内置的多任务系统[，目标是基于 ARM Cortex-M4F 的 MSP432 Launchpad，我们几周前报道过](http://energia.nu/guide/multitasking/)。

[公告贴](http://energia.nu/energia-mt-for-msp432/)给出了几个多任务使用的例子。最简单的是 led 以不同的速率闪烁。如果你想在更接近金属的地方做这件事，你说的是多个定时器，或者单个定时器上的多个比较，也许是一个中断驱动的系统滴答，它有足够高的分辨率来满足你的各种闪烁需求。但是，除非您对这种特定的体系结构非常熟悉，否则设置起来并不容易。Energia 多任务处理将为您处理这些。它基于 [TI 实时操作系统](http://www.ti.com/tool/ti-rtos) (TI-RTOS)，但包装在熟悉的 IDE 中。

UI 让你完全不用考虑硬件。你只需启动一个新的标签并开始编码，就好像你在使用一个完全独立的硬件一样。上面链接的公告帖子提到这些草图是“并行”运行的。嗯……我们知道它不是像 Propeller 那样的多核系统，但我们会顺其自然。这当然比[为这种类型的硬件构建自己的调度器](http://hackaday.com/2014/06/23/multitasking-on-the-msp430f5529-launchpad/)容易。

[感谢 MycoWx]