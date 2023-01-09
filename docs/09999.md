# 简单的 USB 功率计

> 原文：<https://hackaday.com/2015/09/07/simple-usb-power-meter/>

除了数据传输之外，USB 接口越来越多地被用作各种设备的电源和充电端口。在任何黑客工作台上，测量连接到 USB 插座或充电器的设备的电气参数的仪表都很方便。电子实验室的人设计了这个简单的 USB 功率计。

该设备测量电压和电流，并在 0.5 英寸的小型有机发光二极管显示器上显示它们以及计算的功率。该电路是围绕 ATmega328 构建的。为了保持电路板尺寸较小，并减少元件数量，微控制器使用内部 8MHz 时钟。低电阻分流器提供电流感测，该电流感测由 [LT6106 a 高端电流感测放大器](http://cds.linear.com/docs/en/datasheet/6106fa.pdf)放大，然后馈入 ATmega 的 10 位模拟端口。一个 [MCP1525 精密电压基准](http://ww1.microchip.com/downloads/en/DeviceDoc/21653C.pdf)为微控制器的模拟基准引脚提供 2.5V 电压，从而产生 2.44mV 的分辨率。电压测量是通过范围高达 6V 的电阻分压器进行的。Arduino 草图读取模拟端口上的电压和电流数据，并在显示器上显示测量结果。测量数据被平均以滤除噪声。

有机发光二极管显示器有一个 SPI 接口，需要 [u8glib 库](https://code.google.com/p/u8glib/)。该项目使用所有的 SMD 部件，但相当容易手工组装，如果你想尝试表面贴装技术，这可能是一个不错的起步项目。它使用 SolaPCB EDA 软件设计，原理图和电路板布局的源文件以 [ZIP 存档](http://www.electro-labs.com/?wpdmact=process&did=MTIuaG90bGluaw==)的形式提供。下载 BoM 和 Arduino 代码，你就拥有了构建这个漂亮设备所需的一切。

感谢[Abdulgafur]发送此提示。如果你正在寻找一个更全面的解决方案，检查一下令人敬畏的 [Friedcircuits USB 测试器](http://hackaday.com/2015/06/19/review-friedcircuits-usb-tester/)，我们之前评论过它，它在[的 Hackaday 商店](http://store.hackaday.com/products/usb-tester-2-0)有售。