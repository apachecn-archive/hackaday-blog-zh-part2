# RaspiDrums 使用昂贵的传感器

> 原文：<https://hackaday.com/2015/09/04/raspidrums-uses-expensive-sensors/>

压电传感器非常适合用微控制器监控机械冲击。无论你是在监测敲门声还是观察心跳，它们都是完成工作的廉价方式。然而，它们也有缺点，所以当[杰里米]想要制作一套电子鼓时，他决定使用更昂贵的加速度计来测量打击效果。

尽管压电传感器很便宜，但要让它们正常工作还需要大量的工作。[Jeremy]发现的 ADXL377 三轴加速度计所需工作更少，并且由于输出端有 1kHz 低通滤波器，可提供更可靠的数据。在他的设置中，树莓派处理所有繁重的工作。每个鼓上的 ADC 发送关于鼓的每次冲击的数据，Raspberry Pi 通过原生 Alsa 驱动器和 USB 声卡输出声音。

这个项目很大程度上表明，一旦你找到合适的硬件，像这样的项目是多么简单。如果你对在你的最新项目中使用加速度计而不是压电传感器感到好奇，那么[Jeremy]的新电子鼓也有很好的记录。而且，如果你对鼓感兴趣，一定要看看如何在任何地方都能拥有鼓，或者如何打造你自己的逻辑鼓。

[https://www.youtube.com/embed/J-EnJQjJY78?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/J-EnJQjJY78?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)