# 给 Rigol DS1052E 示波器一个频谱分析仪

> 原文：<https://hackaday.com/2012/10/10/giving-the-rygol-ds1052e-scope-a-spectrum-analyzer/>

像许多硬件修理工一样，[dexter2048]在他的工作台上有一台 Rigol DS1052E 示波器。一天，当试图从 FFT 设置中获取一些信息时，[dexter]沮丧地举起双手，决定编写一个具有 FFT 频谱分析的文件查看器。最终的观察器给这个非常强大且便宜的示波器[一个频谱分析仪](http://www.eevblog.com/forum/general-chat/using-rigol-ds1052e-for-spectrum-analysis/)。

[dexter2048]的应用程序能够捕捉 0 Hz 至 500 MHz 的信号，并通过将一根电线插入 Rigol 的一个输入来证明这一事实。产生的波形随后被发送到计算机，在那里[dexter]得到了 82 兆赫和 114 兆赫之间的无线电频谱的清晰图像。在他的图表中，你可以清楚地看到在[德克斯特]的实验室里可以收听到的调频广播电台。

这个对 Rigol DS1052E 示波器的小修改是一长串黑客攻击中的最新一个[，给这个奇妙、廉价的示波器](http://hackaday.com/tag/rigol/)[双倍的带宽](http://hackaday.com/2010/03/31/update-50mhz-to-100mhz-scope-conversion/)，[通过 Python 进行数据收集](http://hackaday.com/2012/03/30/grabbing-data-from-a-rigol-scope-with-python/)，甚至还有一个[自制版本的 Pong](http://hackaday.com/2011/12/31/homebrew-on-the-rigol-ds1052e-scope/) 。任何为旧设备提供新功能的东西对我们来说都是好消息，我们期待未来有更多的 1052E 黑客。

向[Murlidhar]致敬，感谢他送来这个。