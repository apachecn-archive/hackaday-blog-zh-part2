# SDR:卫星死亡接收器

> 原文：<https://hackaday.com/2014/11/04/sdr-satellite-death-receiver/>

万圣节可能已经结束了，但是[happysat]已经找到了一种聆听死者声音的方式。卫星，即 136-138 兆赫和 150-400 兆赫范围内的卫星。他正在使用 RTL-SDR 加密狗和 QFH 天线来探测退役导航和太空研究卫星的垂死挣扎。

[happysat]在 137MHz 波段上收听 NOAA/Meteor 时发现了这一点。当一颗卫星接近寿命终点时，最后一点燃料被用来将它推入墓地轨道。然而，这并不总是有效的，当光线正好时，化学反应会使长期死亡的电池导电，这些炼狱中的卫星再次传输。

他们没有发出任何有用的专有信号，只是未调制的载波，有时会干扰目前在 136-138 MHz 频段上运行的卫星。[happysat]从两颗仍在广播的最老的卫星上捕获了一些音频，并链接到他创建的一组[废弃卫星。检查他的](https://dl.dropboxusercontent.com/u/124465398/tle/deadsat.txt)[频率数据库](https://dl.dropboxusercontent.com/u/43061070/frequencies.xml)的 SDR#以及。没有气象卫星天线？[打造](http://sdrformariners.blogspot.co.nz/2013/08/weather-satellites-antennas.html) [一体](http://www.g4ilo.com/qfh.html)！

[通过[/r/rtlsdr](http://www.reddit.com/r/RTLSDR/comments/2l8y84/receiving_dead_satellites_with_rtlsdr/)