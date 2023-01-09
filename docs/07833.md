# FPGA 流光溢彩克隆包一吨的功能

> 原文：<https://hackaday.com/2014/12/16/fpga-ambilight-clone-packs-a-ton-of-features/>

[Stephen]设计了一个围绕 FPGA 构建的独立流光溢彩克隆，[最近添加了许多新功能](http://hacks.esar.org.uk/hdmi-light-v2/)以使他的设计更好。他的原始设计基于 Spartan 3-E FPGA，但他的新设计使用 Papilio One 板和 Spartan-6 LX9 FPGA。这为他提供了专用 DSP 硬件和更多 RAM，允许他添加更多处理密集型功能。

[Steven]的新主板总共可以驱动多达 4096 个 LED，每个 LED 都是从 256 个分段屏幕区域中的一个区域着色的。led 的输出在一个可配置的时间段内是平滑的，这使得结果更加令人满意。[Steven]还添加了色彩校正矩阵和伽马校正表，以弥补 LED 色彩的差异，因此输出可以根据电视后面墙壁的颜色进行微调。

最后，[Steven]添加了可以存储在闪存中的多种配置。FPGA 可以检测视频流中的信箱和邮筒，并自动更改为相应的配置，因此很少需要手动调整设置。他还添加了一个扩展的串行接口来配置闪存中的所有参数和配置。请务必在休息后观看视频，了解他的设置。

[https://player.vimeo.com/video/114498575](https://player.vimeo.com/video/114498575)