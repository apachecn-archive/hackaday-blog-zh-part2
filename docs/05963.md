# 游戏机大战电子货架标签

> 原文：<https://hackaday.com/2014/05/03/game-boy-vs-electronic-shelf-labels/>

虽然它们在美国可能很少见，但世界上已经有一些大商店开始为商店里的每件商品推出电子货架标签。这些标签确保货架上的每件商品都与商店电脑中的商品价格相同，它们都由悬挂在商店天花板上的红外收发器控制。在研究了其中一个基站后，[furtek]意识到如果你有合适的设备，它们是完全开放的。正确的装备，原来，[是一个游戏男孩色的](http://furrtek.free.fr/?p=crea&a=esl)。

正在讨论的货架标签由基站控制，该基站具有明显非标准的载波频率和专有协议。手机中的红外驱动芯片太慢，无法与这些标签通信，而旧的 PDA 如 Palm Pilots、Zauruses 和 Pocket PCs 只有一个 IrDA 芯片。不过，有一个设备有一个活跃的开发场景和一个直接连接到 CPU 引脚的 IR LED，所以[furtek]开始修补硬件。

Game Boy 需要超频才能获得 1.25 MHz 的正确载波频率。凭借已经在 FPGA 板上开发的概念验证，[furtek]开始为 Game Boy 编写代码，开发一个允许他更改这些电子标签的“页面”或在特定标签上显示定制数据的界面。

这个版本还有一个更重要的含义:这些电子标签的固件可以通过红外更新。所有[furtek]需要的是这些标签中的 uC 开发工具。

有一个很棒的视频[furtek]整理了这个视频。看看下面。

[https://www.youtube.com/embed/YkwY8mwDSec?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/YkwY8mwDSec?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)