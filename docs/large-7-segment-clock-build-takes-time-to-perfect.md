# 大型七段时钟构建需要时间来完善

> 原文：<https://hackaday.com/2015/05/18/large-7-segment-clock-build-takes-time-to-perfect/>

[Kevin Rye]建造了一个基于 TTL 的七段离散时钟，与他为它建造的漂亮外壳相比，他对丑陋的内部不太满意。他开始创造另一个巨大的七段钟放在那个围栏里。

时钟，尤其是基于七段的时钟，并不是什么新鲜的东西。这个仍在进行中的特别项目很有趣。[Kevin]是一名经验丰富的黑客，但他遇到并解决的问题可能有一天会对其他黑客有用。

首先，他试图改变他的旧体形。但用他自己的话说“你可以擦亮一坨屎，但它仍然是一坨屎。”五年后，他受够了。他建造了许多其他的[钟](http://kevinrye.net/files/category-clocks.php)，但是他没有重新利用它们，而是决定从头开始。他很快试验了一台 Arduino 和一些显示器，并使用 [Multiplex7seg](https://code.google.com/p/mutiplex7seg/downloads/detail?name=Multiplex7Seg.zip&can=2&q=) 库驱动它们。那个库只支持四个字符，所以他又回到了起点。有了新的开始，他的设计现在进展顺利。目前，他已经为显示器设计了三块板，两块板用于数字之间的冒号，主 Arduino-clone 控制器板和一个 3D 打印的前框架来支撑显示器。这将是很好的，最终看到围栏接收一些合适的居住者，并使这个建筑关闭。