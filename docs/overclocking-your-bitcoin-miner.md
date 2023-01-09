# 超频你的比特币矿工

> 原文：<https://hackaday.com/2013/08/05/overclocking-your-bitcoin-miner/>

挖掘比特币的游戏名称不是 CPU、GPU，甚至不是 FPGAs。现在，铁杆矿工正在转向定制的 ASIC 芯片，如 Block Erupter，大约 100 美元，你也可以用 2.5 瓦的功率和一个 USB 端口以 300 MH/s 的速度开采比特币。这个速度对于一些人来说是不够的，比如[Jeremy]将他的 Block experter 超频到接近两倍的速度。

[Jeremy]从拆除 Block experter 硬件开始他的教程。在里面，他发现了一个定制的 ASIC 芯片，一个 ATTIny2313，一个 USB UART 转换器和一个用于 ASIC 的稳压器。通过更换连接到 ASIC 的 12 MHz 晶体，并用微调电位计调整电压，[Jeremy]能够将 ASIC 内核从 336 MHz 超频到 560 MHz。实际上，他以一台的价格运行两台 Block expertors，有可能收回购买硬件的成本。

必须指出的是，560 MHz 的数字来自于用 20 MHz 的晶体替换 12 MHz 的晶体，这个 mod 在[Jeremy]的工作台上只持续了大约 20 分钟，直到 magic blue smoke 发布。他建议使用 14 或 16 MHz 的晶体，为稳定的调制解调器提供 392 MHz 或 448 MHz 的新速度。