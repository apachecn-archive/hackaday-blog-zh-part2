# GPIB 转 USB，带有 Python API

> 原文：<https://hackaday.com/2014/05/09/gpib-to-usb-with-a-python-api/>

如果你没有愚蠢到认为基于 Arduino 的示波器和万用表实际上除了最简单的测试和测量之外对所有人都有用，你可能会在你的工作台周围放一些来自 HP 或 Tektronix 的大铁。你可能已经注意到在这些机器的背面有一个奇怪的端口，标记为 GPIB 或 IEEE-488。这是这些设备的标准接口，如果你曾经估算过 USB 到 IEEE-488 转换器的价格，你就能明白为什么[Steven] [认为自己造一个](http://dangerousprototypes.com/forum/viewtopic.php?f=56&t=6120)会更便宜。

这个版本是对我们几年前看到的早期版本的更新。从那以后，[Steven]采纳了社区的一些建议，用合适的 GPIB 线路驱动 IC 替换了一堆电阻，并大体清理了固件。

因为 USB 转 GPIB 适配器只是将这些旧测量设备连接到现代计算机所需工具的一小部分，【Steven】也一直在研究[工具套件](https://github.com/Galvant/InstrumentKit)。这是一个 Python 库，它将所有标准化的仪器命令打包成一个易于使用的 API。你可以在这里查看[仪器套件的文档，或者在 Github](http://instrumentkit.readthedocs.org/en/latest/index.html) 上浏览板卡文件和固件