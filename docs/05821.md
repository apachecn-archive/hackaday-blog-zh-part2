# 使用 RTL-SDR 加密狗和二极管测量频率响应

> 原文：<https://hackaday.com/2014/04/17/measuring-frequency-response-with-an-rtl-sdr-dongle-and-a-diode/>

[Hans]想看看带通滤波器的频率响应，但没有很多测试设备。使用 RTL-SDR 加密狗、一些软件和一个快速制作的噪声发生器，他仍然设法获得了滤波器特性的粗略概念。

他是怎么做到的？他“简单地”测量了带通滤波器连接到其输出端和不连接到其输出端时噪声发生器的频率特性，然后用一条曲线减去另一条曲线。如上图所示，噪声发生器基于一个工作在反向击穿电压下的齐纳二极管。然后用一个简单的电容来实现 DC 阻塞。

鉴于标准 RTL-SDR 加密狗一次只能采样 2-3MHz 宽的频谱间隙，[Hans]使用 [rtlsdr-scanner](http://eartoearoak.com/software/rtlsdr-scanner) 扫描他感兴趣的区域。在他的文章中，他也很好地描述了这种方法的局限性:例如，ADC 的动态范围只有 48dB。