# MobilECG 走向开源

> 原文：<https://hackaday.com/2014/02/23/mobilecg-goes-open-source/>

在一次失败的众筹活动后，[mobile ECG](http://mobilecg.hu/)已经开源。MobilECG 是一款医用 12 导联[心电图仪](http://en.wikipedia.org/wiki/Electrocardiography)。12 导联系统比[过去](http://hackaday.com/2014/02/13/arduino-powered-ecg-informs-users-of-their-death/)中的[ECG](http://hackaday.com/2011/08/03/diy-propeller-based-ecg/)系统要复杂得多。该设备的创始人和设计者[Péter]试图通过 Indiegogo 活动为其筹集资金。虽然 MobilECG 相对便宜，但医疗认证却不便宜。该活动没有达到 23 万美元的目标。[彼得]再次尝试在他的网站上发起一轮草根捐赠。这一轮也没有达到彼得继续从事该项目的目标。为了不让他的努力付诸东流，[彼得]决定向社区发布他的硬件和软件。硬件获得了 CERN OHL 1.2 版[的许可。该软件以幽默的名字](http://www.ohwr.org/licenses/cern-ohl/v1.2) [WTFPL](http://www.wtfpl.net/) 发布。

虽然我们不是 ECG 专家，但基本的硬件设计似乎是合理的。MobileECG 基于德州仪器的八进制模数转换器 ADS1278。使用两个 AVR 微控制器，一个 ATTiny24，一个 ATUC64。模拟设计包含导联脱落检测和除颤器保护等细节。需要注意的是，设计中有一些已知的 bug，[彼得]提到有问题可以联系他。该软件似乎还处于早期阶段，要使它成为最终的设计还需要相当多的工作。虽然我们确实希望[彼得]在他的活动中好运，但我们总是很高兴看到设计发布到开源社区中。

[https://player.vimeo.com/video/76186439](https://player.vimeo.com/video/76186439)