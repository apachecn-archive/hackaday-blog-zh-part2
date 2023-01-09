# 破解 NRF24L01 无线电以获得更大范围

> 原文：<https://hackaday.com/2015/08/15/hacking-a-nrf24l01-radio-for-longer-range/>

[RonM9]对他的 NRF24L01 项目的 50 英尺范围不满意。射频必须穿过四面墙，但对于库存模块，信号在穿过两三面墙后逐渐消失。一个相当简单的[外部偶极天线](http://www.instructables.com/id/Enhanced-NRF24L01/)设法增加了足够的范围来完成这项工作。

[Ron M9]的说明显示了切除现有 PCB 天线的位置，并根据经验调整 24 号线以获得最佳性能。他甚至包括一个基于 Arduino 的测试平台，所以如果你愿意，你可以自己进行测试。

毫无疑问，外置天线将极大地改善无线系统。不过，我们想知道，增加一个长于四分之一波长的地网(在那个频率下，并不算太长)能带来多少好处。业余无线电爱好者经常使用权利来改善受损的天线。另一方面，偶极子有轻微的方向性，所以这也是一个优势。[Ron]指出，如果您同时调整发射机和接收机并排列天线，您将获得最佳性能。

我们已经看到人们只是在天线上钉一根线(见下面的视频)，但这种黑客攻击让我们觉得更有技术含量。如果您想[了解更多关于 NRF24L01 的信息，我们已经在](http://hackaday.com/2013/09/21/sending-data-over-bluetooth-low-energy-with-a-cheap-nrf24l01-module/)之前讨论过了。

[https://www.youtube.com/embed/NpMnauHeR7Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/NpMnauHeR7Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)