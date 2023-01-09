# 使用便宜的 PIN 二极管作为盖革计数器

> 原文：<https://hackaday.com/2014/10/25/use-a-cheap-pin-diode-as-a-geiger-counter/>

福岛核电站灾难后，辐射测量成为许多人的新话题。盖革-米勒管，以前是一件稀奇的东西，现在变得既重要又稀有。

[Opengeiger.de](http://opengeiger.de/) ( [英文版此处](http://opengeiger.de/index_en.html))有完整的制作没有[盖革-米勒管](https://en.wikipedia.org/wiki/Geiger%E2%80%93M%C3%BCller_tube)的盖革计数器的说明。相反，这个计数器使用一个 [PIN 光电二极管](https://en.wikipedia.org/wiki/PIN_diode)和一些精心选择的运算放大器。这种设备的总成本要比其他设备便宜得多:二极管不到 1 美元，其余的大约 5 美元。由于问题中的 PIN 光电二极管用于许多其他设备，它不像盖革管那样是一个利基元件。

秘诀在于元件选择和调整。Opengeiger 使用 BPW34 二极管，因为它相对常见，表面积大，而且反向偏置时电容非常低。第一级运算放大器的选择也相当重要。考虑到平均伽马辐射事件在约 50 微秒内仅产生约 10 毫微安，大量放大(100，000 倍)、低噪声和高带宽是必需的。

如果你想开始这个项目，你可以先浏览一下[解释](http://opengeiger.de/WarumDieseSeite_en.pdf) (PDF)以获得项目目标的概述，[仔细阅读所有的技术考虑](http://opengeiger.de/PinDiodenZaehler_en.pdf) (PDF)或者直接前往[的“斯图加特·盖格尔”](http://opengeiger.de/StuttgarterGeigerleV1_en.pdf)的 DIY 说明(PDF，示意图在最后一页)。所有的文档都充满了相关的参考资料，完全值得一读。