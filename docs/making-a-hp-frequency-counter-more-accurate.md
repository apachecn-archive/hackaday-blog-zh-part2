# 使 HP 频率计数器更加精确

> 原文：<https://hackaday.com/2013/08/26/making-a-hp-frequency-counter-more-accurate/>

[Gerry]为他的 HP 53131 频率计数器构建了自己的[高稳定性时基附加模块](http://gerrysweeney.com/diy-hpagilent-53131a-010-high-stability-timebase-option/ "DIY HP/Agilent 53131A 010 High Stability Timebase Option")。这个项目是在[Gerry]为他的实验室建造了一个[铷 10 MHz 标准](http://hackaday.com/2013/08/05/turning-a-rubidium-standard-into-a-proper-tool/ "Turning a rubidium standard into a proper tool")后开始的。在将标准连接到频率计数器进行校准时，他发现 HP 53131 有一个糟糕的内部振荡器。来自惠普的官方高稳定性时基插件价格约为 1000 美元，他决心做得更好。

利用二手 OCXO 作为振荡器，他设计了自己的附加模块。OCXO 模块将一个晶体振荡器封装在一个热室中。由于温度波动会引起晶体振荡器的漂移，OCXO 控制温度以保持频率恒定。在易贝可以用不到 30 美元买到二手的。

该模块的 PCB 设计可以容纳各种 OCXO 模块。它使用一个高速比较器和一个高稳定性 5 伏基准电压源向计数器提供时钟信号。DAC 用于校准振荡器。通过保持与原始计数器相同的 DAC，可以使用器件的前面板来校准附加板。

该项目是惠普 1000 美元模块的替代产品，成本只是其一小部分。[Gerry]的文章包含了您构建自己的产品所需的所有细节。

[https://www.youtube.com/embed/RPTQaRoiJyE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/RPTQaRoiJyE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)