# 自己造 CPU？那是容易的部分！

> 原文：<https://hackaday.com/2015/07/31/build-your-own-cpu-thats-the-easy-part/>

你想自己造 CPU？那很有趣，但是你可能会发现它并没有你想象的那么难。这些年来，我已经做了几个 CPU，并且不缺少其他的定制 CPU，从非常 T2 严肃的尝试到用 T4 分立芯片制造的计算机，再到用 T6 继电器制造的计算机。不是贬低这种尝试，但真正的问题不是 CPU。它是基础设施。

## 什么样的基础设施？

我认为圣杯会引导你的定制 CPU 进入一个成熟的 Linux 系统。这是一个足够大的工作，我还没有做。虽然你可能比我更有效率，但你可能需要一定的睡眠，所以你可能要考虑一下你是否真的能在合理的时间内完成所有的工作。例如，许多定制的 CPU 不运行交互式操作系统(或者任何操作系统)。在极端的情况下，定制的 CPU 没有任何基础设施，您用直接的机器代码对它们进行编程。

机器码容易出错，所以你真的需要一个汇编程序。如果你在一台大型机器上工作，你甚至可能需要一个连接器。汇编语言编码过一会儿就变得乏味了，所以也许你需要一个 C 编译器(或者其他语言)。调试器？操作系统呢？

每一件事本身都是一个非常严肃的项目(除了制造一个相当强大的 CPU)。除非你或者一个大团队有很多空闲时间，否则你必须考虑如何破解一些捷径。

## 获得基础设施？

得到基础设施最简单的方法就是去偷。但这意味着你的 CPU 必须与其他可用的 CPU 兼容(如 [OpenSparc](http://www.oracle.com/technetwork/systems/opensparc/index.html) 或 [OpenRisc](http://opencores.org/or1k/Main_Page) )，这有什么意思呢？尽管如此，互联网上仍然充斥着以这种方式工作的克隆 CPU。克隆 CPU 有什么用？据推测，设计者希望使用特定的处理器，但希望将其与其他项目集成，以产生一个片上系统。当然，有时候，人们只是想模仿旧机器，这也很有趣。

不过，总的来说，开发自己的 CPU 的吸引力在于让它成为你自己的。也许你想尝试奇怪的指令集架构。也许您知道如何最小化处理器延迟。或者你可以像我一样，只想要一台比任何商业替代品更能模拟你思维方式的计算机。如果是，你会怎么做？你可以尝试移植基础设施。这是偷窃和白手起家的中间点。

## 便携选项

便携式装配工有相当多的选择。假设你的处理器看起来不太奇怪，并且你不介意关于标签和符号的传统汇编约定，你可能会考虑 [TDASM](http://www.penguin.cz/~niki/tdasm) 或 [TASM](http://home.comcast.net/~tasm/tasmsum.htm) 。我对此有自己的变化， [AXASM](https://github.com/wd5gnr/axasm) ，在不久的将来我会更多地谈论它。

汇编语言很好，但是你真的想要一种高级语言。当然，您首先会想到移植 gcc，它是一个很棒的 C 和 C++编译器(以及其他一些东西)。有好消息、坏消息和更坏的消息。好消息是，只要您的架构符合一些预定义的概念(例如，至少 32 位整数和一个平面地址空间)，gcc 就是可移植的。坏消息是做一个港口相当困难。最糟糕的消息是只有数量有限的文档，而且很多都已经过时了。

尽管如此，这是可能的。要产生一个交叉编译器，你只需要做三件事:

*   机器描述
*   机器割台
*   一些机器特有的功能

然而，构建它们相当复杂，并且使用类似 Lisp 的符号，这并不总是直观的。如果你想解决它，有几个感兴趣的文件。有很好的[幻灯片概述](http://gcc.gnu.org/ml/gcc-help/2004-10/msg00060/GccPorting.pdf)，[很过时的官方文件](https://gcc.gnu.org/onlinedocs/gcc-3.0.4/gcc.html)，还有[某家伙的硕士论文](http://monarch.qucosa.de/fileadmin/data/qucosa/documents/4857/data/thesis.pdf)。然而，也要做好阅读大量源代码和实验的准备。然后你可能还想移植 gdb，这也是很重要的(见下面的视频)。

[https://www.youtube.com/embed/kgFr4Jnhff0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kgFr4Jnhff0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

还有其他的 C 编译器。llvm 项目有 clang，你可能会发现它稍微更容易移植，尽管它仍然不是我认为微不足道的。 [lcc](https://github.com/drh/lcc) 编译器在 1995 年作为一本书问世。它使用 [iburg](https://github.com/drh/iburg) 来进行代码生成，该工具可能对其他一些重定向项目也有用。虽然 [vbcc](http://www.compilers.de/vbcc.html) 编译器不经常更新，但它的后端文档看起来非常好，似乎是更容易移植的编译器之一。有一个可移植的 C 编译器， [PCC](http://pcc.ludd.ltu.se/) ，是相当值得尊敬的。我见过有人将一些“[小 C](http://www.drdobbs.com/developer-network-small-c-compiler-book/184415519) ”变体移植到不同的 CPU 上，尽管因为它们不是标准 C，所以用途有限。

请记住，进行 gcc 移植不仅仅是 C 编译器的事情。你需要定义你的 ABI(应用程序二进制接口；基本上是如何组织内存和传递参数的)。您还需要提供至少一些引导 C 库，尽管在让编译器工作之后，您可能能够重新利用许多标准库。

所以可能 C 编译器有点多。还有其他方法可以让高级语言运行起来。生产一个可工作的 JVM(或其他虚拟机)将允许你交叉编译 Java，并且可能总体工作量更少。尽管如此，这仍然不容易，你的 JVM 的性能甚至可能无法接近一个编译过的程序。我发现 Forth 的版本很容易上手。如果你能找到它的备份，那么第四集的琼斯是一个很好的起点。

如果你真的咬紧牙关构建了一个 C 编译器，操作系统就是下一个障碍。大多数 Linux 版本都假设您拥有像内存管理这样的高级特性。有一个版本， [uClinux](http://www.uclinux.org/) ，可能更容易移植。你最好看看像[孔蒂基](http://contiki.sourceforge.net/docs/2.6/)或[弗里托斯](http://www.freertos.org/)这样的东西。

## 一个现实主义镜头

构建一个新的 CPU 并不适合胆小的人，可能也不是你第一个 FPGA 项目的最佳选择。有时，仅仅获得一个像样的前面板就可能是一个挑战(见下面的视频)，更不用说编译器和操作系统了。

[https://www.youtube.com/embed/dt4zezZP8w8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/dt4zezZP8w8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

对于一个黑客来说，把一个新系统引导成一个完全运行 Linux 的庞然大物需要做大量的工作。它可能更适合一群黑客。也许你可以在 [Hackaday.io](https://hackaday.io/) 上主持你的项目。

尽管如此，仅仅因为你不能在一个周末制造下一个 128 位超标量 CPU，并不意味着你不应该尝试制造一个 CPU。你会学到很多东西，谁知道呢，你甚至可能会发明一些新东西。