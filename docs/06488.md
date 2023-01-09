# 覆盖受保护的 AVR 引导程序

> 原文：<https://hackaday.com/2014/07/05/overwriting-a-protected-avr-bootloader/>

[![Logo for the FIgnition 8 bit computer project](img/03d2e1868368ff6b2d469117a31c318f.png)](http://hackaday.com/?attachment_id=126096)

引导加载程序通常用于更新微控制器上的应用程序代码。它从主机接收新程序，将其写入闪存，验证程序是否有效，并复位微控制器。也许最普遍的例子是 Arduino bootloader，它允许你在没有 AVR 程序员的情况下加载代码。

引导装载程序驻留在内存中受保护的特殊部分。在 AVR 上，不可能从应用程序代码写入引导装载程序内存。这是为了防止您意外破坏引导加载程序并阻塞设备。

但是，写入引导加载程序内存会很有用。最好的例子是当你需要更新引导程序本身的时候。为了做到这一点，[Julz]找到了一个解决办法，即[击败了 AVR 引导程序保护](http://oneweekwonder.blogspot.co.uk/2014/07/bootjacker-amazing-avr-bootloader-hack.html)。

挑战在于找到一种方法来执行存储程序存储器(spm)指令，该指令只能由引导装载程序执行。[Julz]通过计算周期并在适当的时候修改寄存器，成功地利用了现有 bootloader 中的 spm 指令。

使用这种[Julz]称为 BootJacker 的技术，[配置 8 位计算机](https://sites.google.com/site/libby8dev/fignition)可以更新它的引导装载程序。但是，这种技术可能允许您修改 AVR 设备上的大多数引导加载程序。