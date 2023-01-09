# 对 Lattice 的 ICE40 FPGA 比特流进行逆向工程

> 原文：<https://hackaday.com/2015/03/29/reverse-engineering-lattices-ice40-fpga-bitstream/>

与微控制器项目不同，涉及 FPGAs 的项目还不能声称依赖于成熟的开源工具链。在某种程度上，每个 FPGA 都需要配置由封闭源合成工具产生的专有比特流。缺乏完整的 FPGA 工具链来将您的项目从 Verilog-或-VHDL 转换为可上传的比特流是由多种原因造成的。首先，编写这样的“编译器”是复杂的。它涉及对 FPGA 上可用资源的深入了解，这些资源可以吸收目标设计的功能。其次，整个合成过程是闭源的，对每个 FPGA 供应商来说都是一种“秘方”。

作为回应，[Alex]和[Clifford]已经向一个 FPGA 的开源工具链迈出了第一步；他们已经对 Latttice Semiconductor 的 iCE40 FPGA 进行了逆向工程。两人并不是一时兴起选择了 iCE40。这一选择是有意的，因为 FPGA 在开发板上[售价仅为 22 美元，所以其他人可以跟随他们的脚步而不会破产。](http://www.latticesemi.com/icestick)

在下面的视频中，[Clifford]演示了这种新工具的功能，将设计从 Verilog 合成为比特流，然后再从比特流合成回 Verilog。考虑到这一特性，已经做了大量的工作来为这个特定的 FGPA 开发一个完美的开源工具链。

要获得最新代码的副本，请看一下它的[文档页面。](http://www.clifford.at/icestorm/)

[https://www.youtube.com/embed/u1ZHcSNDQMM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/u1ZHcSNDQMM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)