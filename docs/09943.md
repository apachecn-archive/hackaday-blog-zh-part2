# 在试验板上前进

> 原文：<https://hackaday.com/2015/08/30/go-forth-on-a-breadboard/>

Forth 并不是一种闪亮的新编程语言，但它有一批坚定的追随者，因为它是轻量级的和优雅的。这是[查克·摩尔]的心血结晶，语言看似简单。单词是由空格分隔的字符序列。最简单的形式是，Forth 知道几个基本单词，包括——这是关键——一个定义其他单词的单词。

[Jean-Claude Wippler]喜欢试验物理计算，他[找到了第四张为 LPC1114](http://jeelabs.org/2015/07/22/forth-on-a-dip/) 准备的图像。为什么会有意思呢？LPC1114 是少数(或者可能是唯一)采用试验板友好 DIP 封装的现代 ARM 处理器之一。因为[吉恩-克劳德]有一个芯片，他很快就有了第四个系统。他只需要一块试验板和一个 3.3V 串行连接器。该芯片有自己的引导程序，他使用的 [Mecrisp-Stellaris](http://mecrisp.sourceforge.net/) Forth 有超过 300 个单词，当然还有能力添加更多。

如果你曾经使用过惠普计算器(或计算尺)，你会发现 Forth 使用了反向波兰符号(RPN)。例如，以下单词计算并打印 2 乘以 10:

```
10 2 * .
```

您可以像这样造一个词来将事物乘以 2(例如，mydouble ):

```
: mydouble 2 * ;
```

所以你可以说

```
10 mydouble .
```

这看起来很简单，但是你可以为 Forth 本身构建很多这样的东西，包括完整的汇编器，甚至交叉编译器。

顺便说一下，相同的 Mecrisp-Stellaris Forth 将在我们几周前报道的 [KL25Z mbed 板](http://hackaday.com/2015/08/11/getting-started-with-arm-using-mbed/)上运行。你甚至可以在 Arduino 上跑步(见下面的视频)。如果你买了一个冰棍来跟随我们最近的 [FPGA 教程系列](http://hackaday.com/2015/08/19/learning-verilog-on-a-25-fpga-part-i/)，你也可以[在那块板上运行第四个 CPU](http://hackaday.com/2015/07/28/open-source-fpga-toolchain-builds-cpu/)。

[https://www.youtube.com/embed/klDKTS7iEQU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/klDKTS7iEQU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)