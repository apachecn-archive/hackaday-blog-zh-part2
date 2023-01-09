# 200 LED 环形钟

> 原文：<https://hackaday.com/2014/06/24/the-200-led-ring-clock/>

有 LED 钟，然后还有 30 步外就能致盲的 LED 钟。LED 挂钟就是后一种。200 个 ws 2812 b/neo pixel RGB led 将环形时钟驱动到瞳孔灼热的水平。时钟运行在 ATMega1284P 上，计时由[恩智浦 PCF8563](http://www.nxp.com/products/interface_and_connectivity/i2c/i2c_real_time_clocks_rtc/series/PCF8563.html) 实时时钟芯片处理。代码是使用 Adafruit 的 Neopixel 库用 Arduino 的接线语言编写的。

用一块印刷电路板(PCB)制造时钟既昂贵又浪费。[stigalicious]巧妙地设计了他的时钟，用 8 个相同的 PCB 复制而成。每块板构成了环的 45 个饼图部分。所有 8 个 PCB 都有 CPU、时钟芯片和其它各种分立器件的封装，但只有“主”部分有这些器件。7“从”部分简单地通过每个 LED 传递时钟、数据、电源和接地。他使用 Seeedstudio 的电路板服务制作了 10 份 PCB，以防出现任何错误。

[stigalicious]孤注一掷，购买了他需要的 200 个 led。要么他真的很幸运，要么 WS2812 质量测试有所改善，因为只有一个 LED 有一个死蓝色的 LED。

如果你想了解更多信息，[stigalicious]在他的 [Reddit 帖子](http://www.reddit.com/r/electronics/comments/28ums7/i_made_an_rgb_led_clock_not_my_first_project_but/)中提供了大量细节。他没有为时钟设置网页，但他上传了他的[源代码](http://pastebin.com/cqEA944g) (pastebin 链接)和 [Altium 原理图/PCB 文件](https://mega.co.nz/#!1dYQgbKB!siYEBrqhNGCAOx_u1cmpyJjxIO0ZfKkkimc6TglbKlo[1]) (mega.nz 链接)。我们可能有点偏见，但 [hackaday.io](http://hackaday.io/) 将是这个项目或任何其他项目的完美地点！