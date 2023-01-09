# 用 Python 编程 FPGAs

> 原文：<https://hackaday.com/2012/06/11/programming-fpgas-with-python/>

![](img/2a18ca3eac2b3ff469f12027562f91ec.png "Py")

如果你曾经想进入 FPGA 的世界，但又不想学习另一种语言，你现在可以用 Python 编程一个 [FPGA。PyCPU 将非常非常简单的 Python 代码转换成 VHDL 或 Verilog。由此，可以将硬件描述上传到 FPGA。](http://pycpu.wordpress.com/)

PyCPU 支持的 Python 语言部分是 *[极度](http://pycpu.wordpress.com/info/supported-python-code/)* [极小](http://pycpu.wordpress.com/info/supported-python-code/)，只有 *int* s 是唯一支持的内置数据类型。当然 *if* s 和 *while* s 仍然包含在所有的赋值和操作符中。一个新的补充是用 Python 获得数字 IO 访问的方法，如果你打算编程芯片，这是一个明显的要求。

PyCPU 肯定不会很快取代 VHDL 或 Verilog，但如果你正在寻找进入 FPGAs 和它提供的“告诉芯片什么是”范例，它肯定是一个值得研究的工具。

向[hardsoftlicus]致敬，感谢他发来这封信。我们的精彩(我们的意思是，真的)注意到一些错误时，这是第一次张贴。那些错误已经被改正了。