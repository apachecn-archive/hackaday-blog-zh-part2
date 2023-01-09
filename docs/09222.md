# 用 Linux 控制一个 Rigol

> 原文：<https://hackaday.com/2015/06/06/controlling-a-rigol-with-linux/>

Rigol DS1052E 是任何修补工作台的事实上的示波器。它便宜，它够好，它已经存在很久了；现在有了新的 1054 zed 型号，你甚至可以买到便宜的 1052E。

[wd5gnr1]想出了一个非常有趣的软件，它允许 Linux 系统控制这个流行示波器上的大多数功能。只需一根 USB 线，就可以读取和记录示波器的所有测量值，以 CSV 格式保存波形，并将数据发送到 gnuplot 和 qtiplot。

由于 1052E 已经存在了很长一段时间，所以有很多软件利用了这个示波器前面漂亮的 USB 端口。如果你需要一个便宜的频谱分析仪，[给你](http://hackaday.com/2012/10/10/giving-the-rygol-ds1052e-scope-a-spectrum-analyzer/)和工具。这个范围[的本地 WFM 文件甚至存在于 Windows](http://hackaday.com/2013/03/25/rigol-wfm-viewer-ported-for-non-windows-users/) 中。[wd5gnr1]甚至说他的工具很可能可以移植到 Windows 上，但“就用 Linux 吧。'