# 精确测量电导率

> 原文：<https://hackaday.com/2014/11/10/accurately-measuring-electrical-conductivity/>

[Ryan] [设计了一个 PCB](https://www.sparkyswidgets.com/portfolio-item/miniec-i2c-ec-interface/) ，可以让你轻松地从 I2C 上空的一个商用电导探针上获取读数。[电导率测量](http://en.wikipedia.org/wiki/Conductivity_%28electrolytic%29)非常适合测量溶液的盐度，这对于溶液培养等应用非常有用。虽然探针本身有点贵(易贝的价格在 50 美元左右)，但它们非常准确，而且耐用。

商用电导探针包含铂电极以防止腐蚀。用交流信号激励电极，这防止了溶液的极化并避免了电极上的化学反应。当电极被激励时，测量两个电极之间的电压，该电压与溶液的电导率成比例

[Ryan]的电路板产生+/-5v 电压，并使用一个[文氏电桥振荡器](http://en.wikipedia.org/wiki/Wien_bridge_oscillator)产生一个正弦波来激励最外面的电极。电极两端的电压被放大并馈入 MCP3221，这是一款廉价的 12 位 ADC，具有 I2C 接口。[Ryan]还为 MCP3221 编写了一个 [Arduino 库](https://github.com/SparkysWidgets/MCP3221-Library)，这样你就可以很容易地启动并运行你的探测器。