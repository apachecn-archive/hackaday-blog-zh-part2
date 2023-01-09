# 为 ESP8266 编译您自己的程序

> 原文：<https://hackaday.com/2014/12/08/compiling-your-own-programs-for-the-esp8266/>

当 ESP8266 首次向世界公布时，我们震惊地发现有人能够制作一个廉价、可访问的 UART 到 WiFi 桥。在我们获得一些开放的频谱和更好的硬件之前，这是构建物联网所需的部分。

然而，它并没有就此停止。一些非常聪明的人发现 ESP8266 板上有一个相当高功率的微控制器，大量的闪存和大量的 RAM。看起来你可以把 ESP8266 作为它自己的控制器；有了这个芯片，你所需要做的只是为 ESP 写一些代码，你就有了一个完整的解决方案，可以让你的互联网连接的闪光灯或支持 WiFi 的烤面包机。我想，不管现在酷孩子在做什么时髦的事情。

但是，如何为 ESP8266 设置工具链呢？你如何建立项目？你怎么上传这东西的？是的，很复杂，但永远不要害怕；[【CNLohr】在此为您提供便利](https://www.youtube.com/watch?v=pWo-ErpVZC4)。他制作了一个视频，介绍了运行工具链、设置构建环境以及在 ESP8266 上放置一些代码的所有步骤。[都在 git](https://github.com/cnlohr/ws2812esp8266) 里了，还有一些视频注解。

本教程涵盖了设置 Xtensa 工具链和 GCC、GDB 和 binutils 的补丁版本。这将需要很长很长的时间来构建，但一旦完成，您就有了 ESP8266 的构建环境。

将构建环境放在一起，[CNLohr]然后从官方网站获取 Espressif SDK，并将示例图像放在一起。[上传到模块](https://github.com/esp8266/esp8266-wiki/wiki/Uploading)需要拉高一些引脚和拉低一些引脚，插入 USB 转串行模块以将代码发送到模块，退后一点，然后按下上传。

对于他的示例图像，[CNLohr]有几个 WS2812 RGB LEDs 连接到 ESP8266 WiFi 模块。上传图像会将 led 变成可以通过端口 7777 上的 UDP 数据包进行控制的东西。这正是你想要的可编程 WiFi 芯片，这只是这个非常酷的模块可以做什么的开始。

如果你正在寻找某种带有 ESP8266 的开发板，[Mathieu] [一直在玩一些很酷的板](http://www.limpkin.fr/index.php?post/2014/12/07/First-Steps-with-the-ESP8266-03-Development-Board)，我们一直在研究制作一个 Hackaday 版本在商店里销售。Hackaday 版本很可能不会发生，因为 FCC。

[https://www.youtube.com/embed/pWo-ErpVZC4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/pWo-ErpVZC4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

**编辑**:【CNLohr】指出有一个[更受欢迎的工具链](https://github.com/esp8266/esp8266-wiki/wiki/Toolchain)，大多数人都转而使用它。