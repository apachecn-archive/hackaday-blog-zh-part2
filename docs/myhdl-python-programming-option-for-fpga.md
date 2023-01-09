# 面向 FPGA 的 MyHDL Python 编程选项

> 原文：<https://hackaday.com/2012/06/13/myhdl-python-programming-option-for-fpga/>

MyHDL 是一个 Python 模块，它将 FPGA 编程引入了 Python 环境。[Christopher Felton]向我们透露了他刚刚完成的一个简单教程，该教程概述了该模块的使用方法。

你可能还记得几天前听说的 py CPU T1，它可以在 FPGA 上运行非常简单的 Python 代码。在评论区有一个比较 PyCPU 和 [MyHDL](http://www.myhdl.org/) 的健康讨论。虽然它们初看起来很相似，但两者有很大的不同。PyCPU 在 FPGA 芯片上创建了一个处理器，可以执行小范围的 Python 代码。MyHDL 实际上在 Python 环境中实现了硬件描述语言。一旦您使用 HDL 在 Python 脚本中对您的硬件选择进行建模，它就会被转换为 VHDL，然后被馈送到工具链，并像平常一样被推送到芯片。

这不是绝对的初学者体验。但是，如果你精通 Python，那么跳到 HDL 会容易得多，因为你将使用你已经熟悉的语法。