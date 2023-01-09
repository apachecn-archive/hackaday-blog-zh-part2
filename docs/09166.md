# ICE40 FPGAs 的开源工具链

> 原文：<https://hackaday.com/2015/05/29/an-open-source-toolchain-for-ice40-fpgas/>

FPGAs 很棒，但是开源就不行了。FPGA 领域的所有参与者都有自己的专有工具来创建比特流文件，并且为任何 FPGA 合成您选择的 HDL 通常意味着同意没有人阅读的条款和条件。

经过几个月的工作，并基于[Clifford Wolf]和[Mathias Lasser]之前的工作，[Cotton Seed]发布了一个完全开源的 Verilog 到 bitstream 开发工具链，用于 Lattice ice 40 LP，支持更多正在开发的设备。

去年三月，我们看到了对 Lattice ICE40 比特流的逆向工程，但这与一个健壮、成熟的开发平台相去甚远。与同样由 Clifford Wolf 编写的 [Yosys](http://www.clifford.at/yosys/) 一起，从 Verilog 到运行自己代码的 FPGA 相对简单。

下面是视频演示，在冰风暴项目页面上有大量的文档。你也可以花大约 22 美元买到[相关的开发板。](http://www.latticesemi.com/icestick)

[https://www.youtube.com/embed/yUiNlmvVOq8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/yUiNlmvVOq8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)