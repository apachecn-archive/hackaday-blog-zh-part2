# 使用电视调谐卡运行软件定义的收音机。

> 原文：<https://hackaday.com/2012/03/30/working-software-defined-radio-with-a-tv-tuner-card/>

[巴林特·塞伯]刚刚提交了一个他一直在做的小而及时的项目:一个用于 Realtek RTL2832U 的软件无线电[源模块。现在，有了廉价的 USB 电视调谐器卡，您就可以直接进入软件定义的无线电世界。](http://wiki.spench.net/wiki/Gr-baz#rtl_source_c)

就在一周前， [hackaday](http://hackaday.com/2012/03/20/software-defined-radio-from-a-usb-tv-capture-card/) 和[其他媒体](http://dangerousprototypes.com/2012/03/20/introducing-rtl-sdr-a-20-sdr)发布了关于使用 20 美元的 USB 电视捕捉加密狗进行软件无线电的故事。当时，这些采集卡只能将数据直接写入文件。有了[巴林特]的工作，任何人都可以使用带有[HDSDR](http://www.hdsdr.de/)、[Winrad](http://www.winrad.org/)或[GNU Radio](http://gnuradio.org/)的廉价电视调谐器加密狗。如果您曾经考虑过尝试软件定义无线电，现在可能正是时候。

在互联网上的其他地方，一个令人惊讶的活跃的 RTL-SDR 子编辑器出现了，它致力于将 Realtek RTL2832U 调谐器用于软件定义的无线电。有一个[可怕的兼容性图表](http://www.reddit.com/r/RTLSDR/comments/rbqfz/rtlsdr_compatibility_list_work_in_progress_please/)列出了兼容的 USB 加密狗。最便宜的(到目前为止，可能会有变化)是易贝上售价 11 美元的 Unikoo UK001T。

有了他的信号源模块，[巴林特]可以收听 64-1700 兆赫之间的任何广播。采样深度为 8 位，采样速率最高可达 3.2 MHz。休息之后，你可以观看[巴林特]测试他的 20 美元 GNU 无线电设备。

[https://www.youtube.com/embed/FUQd9HOVTk8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FUQd9HOVTk8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)