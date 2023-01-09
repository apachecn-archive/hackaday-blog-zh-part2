# 《瓦特计制作》带您了解功率测量基础知识

> 原文：<https://hackaday.com/2015/02/07/watt-meter-build-walks-you-through-power-measurement-basics/>

你几乎从未听说过 DC 瓦特计——人们只是在脑后用伏特和安培做一些心算。另一方面，交流瓦特计在任何工作台上都非常有用。这款方便的 DIY 数字交流瓦特计不仅具有令人印象深刻的 30A 电流范围，而且采用手持式设计，便于随身携带。

来自 Electro-Labs 的设计为硬件提供了构建指令，并为其核心 PIC 微控制器提供了软件。详细的描述将带您了解原理图的各个模块，此外还有一些交流功率测量的基础知识。原理图和电路板布局是使用 [SolaPCB](http://www.fabstream.com/solopcb-design-software.php "SolaPCB") 完成的——这是一款我们到现在才听说的 Windows 专用免费 EDA 工具。完整的 BoM 和 PIC 代码完善了构建。在硬件方面，该单元使用带有 SPI 接口的 [MCP3202 12 位 ADC 转换器，使其易于连接到微控制器。一个简单的电阻分压器和一个基于 ACS-712 霍尔效应的线性电流传感器 IC](http://ww1.microchip.com/downloads/en/DeviceDoc/21034D.pdf) 是主要的传感元件。相位计算由微控制器完成。隔离的重要性不容忽视，使用光隔离器使数字部分远离模拟部分。电路板轮廓看起来像是被设计成适合一些现成的手持式塑料外壳(如果你找不到，就从 3D 打印机中快速制作一个)。

虽然该设计适用于 230V~250V 范围，但通过改变几个部件，它可以很容易地修改为 110V 使用。交换变压器，改变电阻分压器值，也许一些 DC 电平转换，你就可以了。除了功率之外，这款电表的一个很好的升级功能是能量测量。要深入了解传统电能表的工作原理，请观看视频[【Ben Krasnow】解释千瓦时表](http://hackaday.com/2013/10/10/ben-krasnow-explains-kilowatt-hour-meters/)