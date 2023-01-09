# 适合埃尔莎女王冰雪宫殿的二进制时钟

> 原文：<https://hackaday.com/2015/01/16/binary-clock-fit-for-queen-elsas-ice-palace/>

当生活给你柠檬，你就做柠檬水。当生活给了你冰冷的温度和满院子的雪，你用冰做了二进制时钟。至少丹尼斯是这么做的。

[丹尼斯的]钟是由几个圆柱形冰块堆叠而成的。有六列冰块。这些块状物是通过将水倒入空的人造黄油容器中并冷冻制成的。一旦它们被冷冻起来，[丹尼斯]在每块积木的底部钻了一个 5/16 英寸的洞来放置一个 LED。电线从发光二极管回到冷却器的排水口。

冷却器中装有主要的电子设备。LED 控制板是[丹尼斯]自己设计的。它包含六个 TLC59282 芯片，允许控制多达 96 个 led。每个芯片的输出线连接到两个 RJ45 连接器。[Dennis]不能只使用一个，因为连接器中的八根电线中有一根被用作公共电源线。主 CPU 是一个 Arduino。它连接到一个 DS3234 实时时钟，以保持准确的时间。振荡器监测温度，以便即使在严冬也能保持准确的时间。

[https://www.youtube.com/embed/uddz6QNM6pg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/uddz6QNM6pg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)