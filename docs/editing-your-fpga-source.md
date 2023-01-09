# 编辑您的 FPGA 源代码

> 原文：<https://hackaday.com/2012/07/22/editing-your-fpga-source/>

![](img/3d372dfddc07585199e0cf9283524e94.png "FPGA")

[Dave]指出，在最近对 FPGA 开发人员的调查中，emacs 无疑是最受欢迎的 VHDL 和 Verilog 编辑器。这有几个原因——也就是说，emacs 附带了用于编辑您选择的 HDL 的包。对于我们这些不想安装(和学习)emacs 操作系统的人，[Dave] [用 Notepad++来处理这些包。](http://www.fpgarelated.com/showarticle/37.php)

Notepad++已经有了 VHDL 和 Verilog 高亮显示以及其他高级文本编辑器特性，但是[Dave]想要模板、自动声明和美化。为了做到这一点，他使用[手指文本](https://github.com/erinata/FingerText)将代码存储为片段，并在手指一挥时调用它们。

在[Dave]编写代码时，组件声明需要不断更新，在 Perl 脚本的帮助下，[Dave]可以通过点击热键来更新它们。美化更难，因为 Notepad++甚至没有 VHDL 或 Verilog 美化器插件。这是通过安装 emacs 并作为批处理脚本运行美化过程来实现的。没有人能拥有一切，但我们认为[Dave]摆脱 emacs 的方法非常巧妙。