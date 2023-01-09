# FPGA 控制的回流焊炉

> 原文：<https://hackaday.com/2013/12/28/a-fpga-controlled-reflow-oven/>

圣诞节，[仓鼠]的妻子送给他一个迷你烤箱。那天晚些时候，他把它拆开，造了这个 [FPGA 控制的回流焊炉](http://hamsterworks.co.nz/mediawiki/index.php/Reflow_Oven "FPGA Reflow Oven")。

我们在过去已经看到了很多[回流](http://hackaday.com/2012/01/01/a-very-detailed-reflow-oven-build/) [烤箱](http://hackaday.com/2012/03/08/toaster-oven-reflow-soldering-roundup/)的建造。这些项目大多使用微控制器进行闭环控制，感应温度并触发加热元件达到设定值。该构建使用 [Papilo One](http://papilio.cc/) FPGA 开发板作为控制器。它实现了满足焊膏回流曲线的状态机，确保 SMD 元件焊接正确。

烤箱使用 [MAX31855](http://www.maximintegrated.com/datasheet/index.mvp/id/7273) 从热电偶读取温度。该器件提供放大、冷结补偿和模数转换功能，可通过 SPI 输出温度。为了控制加热器，使用 40A 固态继电器。

驱动这个烤箱的 VHDL 代码在文章中有链接，对于那些想尝试 FPGAs 的人来说有一些有趣的内容。它包括一个 SPI 接口、显示驱动器和温度状态机逻辑。