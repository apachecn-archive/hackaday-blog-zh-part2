# Altoids Tin 网络分析仪

> 原文：<https://hackaday.com/2015/02/09/altoids-tin-network-analyzer/>

网络分析仪常用于测量滤波器，这使得它们对于构建无线电和一般的 RF 应用非常有价值。然而，它们非常昂贵。[然而，你可以在一个 Altoids 罐中用一个 Arduino Nano、一个小屏幕和一个在易贝获得的 AD9850 频率合成模块建造一个](http://soldersmoke.blogspot.com/2015/02/duwaynes-scalar-network-analyzer-in.html)。

网络分析仪的基本思想是将频率馈入器件，测量器件输出的幅度，并绘制频率关系图。[Bill Meara]之前做过以人为本的网络分析仪，手工改变频率，绘制被测设备的输出。[DuWayne] (KV4QB)建立一个设备，使整个过程自动化。

框图非常简单，AD9850 向器件发送信号，由 Arduino 利用一个小放大器进行测量。当信号从被测设备返回时，再次被测量，所有这些被绘制在一个小显示器上。简单，而且[DuWayne]在一个小型无焊试验板上制作的低通滤波器和晶体滤波器获得了一些非常好的读数。