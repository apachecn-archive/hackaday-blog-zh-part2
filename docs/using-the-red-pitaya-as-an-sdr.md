# 使用红色火龙果作为特别提款权

> 原文：<https://hackaday.com/2015/03/02/using-the-red-pitaya-as-an-sdr/>

Red Pitaya 是一个信用卡大小的主板，运行 Linux，有以太网和大量 RAM。这听起来很像树莓皮和比格骨黑，但相似之处仅此而已。红色火龙果还有两个 RF 输入、两个 RF 输出和一个数字 io 负载，所有这些都连接到一个包含 FPGA 的 Xilinx SoC。[Pavel]意识到火龙果拥有软件定义无线电的所有组件，[并构建了一个实现来证明这一点](http://pavel-demin.github.io/red-pitaya-notes/sdr-receiver/)。

SDR 的输入通过一个由电话线制成的简单环形天线直接接入高阻抗输入之一。这种无线电的实际软件定义部分大量借鉴了 Xilinx 应用笔记中的[，而一切都由](http://www.xilinx.com/support/documentation/application_notes/xapp1113.pdf) [SDR#](http://sdrsharp.com/#download) 或 [HDSDR](http://www.hdsdr.de/) 控制。

[Pavel]在他的所有软件中都包含了一个预先构建的 SD 卡映像，因此克隆这个项目只是简单地复制一个 SD 卡并构建一个天线。完整的源代码也是可用的，如果你想了解 FPGAs 和 SDR，这很有趣。