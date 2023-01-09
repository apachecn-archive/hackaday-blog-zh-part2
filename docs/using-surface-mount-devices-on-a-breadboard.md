# 在试验板上使用表面贴装器件

> 原文：<https://hackaday.com/2014/07/25/using-surface-mount-devices-on-a-breadboard/>

[Czar]正在使用 MCP3008 模数转换器进行一个关于 Raspberry Pi 的项目。这种芯片的表面贴装 SOIC 版本稍微便宜一些，而且总有办法让它工作。*T5【沙皇】如何做到这一点令人印象深刻，因为它比通孔版本更灵活，如果做得正确，是一个非常坚固的黑客。*

一些新的引线需要焊接到 SOIC 封装上，为此[沙皇]选择了跳线。这使得每个引脚都很容易插入无焊试验板，而且由于[Czar]非常聪明，所有电源线、地线、模拟线和 SPI 线都有颜色编码。

简单地在芯片上焊接几根跳线不会持续很长时间。为了解决这个问题，[Czar]用热胶封装了整个芯片及其连接。可能不是最好的解决方案，重型环氧树脂会更好，但目前的构建足以承受工作台上相对较小的滥用。