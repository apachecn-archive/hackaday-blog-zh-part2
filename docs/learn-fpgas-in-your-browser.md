# 在浏览器中学习 FPGAs

> 原文：<https://hackaday.com/2015/07/21/learn-fpgas-in-your-browser/>

FPGAs 并没有真正被编程，它们是被配置的。大多数设计人员使用 Verilog 或 VHDL 来描述所需的电路配置。开发人员通常会在将这些配置应用到芯片上之前对其进行模拟(这是一个好习惯，尤其是当你从 FPGAs 过渡到 ASICs 时，这种改变是非常昂贵的)。这种模拟需要你安装和学习很多软件，对吗？

不一定。您可以在浏览器中处理电子邮件、文字处理和 PCB 布局。[为什么不是 FPGA 设计](http://www.edaplayground.com)？EDAPlayground 网站提供了两个编辑器视图:一个用于您的主“代码”，另一个用于 testbench(您用来测试您的设计的模拟驱动程序)。如果你有一个复杂的设计，你甚至可以打开多个文件。

一旦你输入你的 Verilog 或 VHDL(或者从许多例子中选择一个)，你就可以运行模拟并在你的浏览器中看到结果。无需安装软件，除了实际学习 VHDL 或 Verilog 之外，没有太多的学习曲线。

正如[Strauburn]、[combinary logic]和其他人对我们最近关于 VHDL CPU 的帖子的评论，你可以在没有接触到真正的硬件的情况下做很多学习。该网站为您提供了几个不同的工具(如果您想了解您的代码在不同工具上的表现，这很有用)以及许多标准的验证库。综合工具有限，但老实说，如果你想开发真正的硬件，你需要针对你所使用的特定 FPGA 的供应商工具。

至于学习 FPGA 开发的实际艺术，在网上或 YouTube 上快速搜索 Verilog 教程或 VHDL 教程会让你入门。Verilog 很像 C，VHDL 更像 Ada，相应选择。如果你渴望 VHDL，用 [Free Range Factory 的免费书](http://freerangefactory.org/books_tuts.html)不会错。对于 Verilog，[这个列表](http://verilog.comuf.com/docs.html)将让你开始。

[https://www.youtube.com/embed/NXlqdrYga9M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NXlqdrYga9M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)