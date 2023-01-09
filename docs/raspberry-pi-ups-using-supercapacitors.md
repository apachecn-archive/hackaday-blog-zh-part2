# 使用超级电容器的 Raspberry Pi UPS

> 原文：<https://hackaday.com/2014/04/03/raspberry-pi-ups-using-supercapacitors/>

当你想把一个 Raspberry Pi 集成到一个由电源电压控制开关的项目中时，会发生什么呢？是单独给 Pi 供电，还是给它做一个 [UPS？](http://www.hackerspace-ffm.de/wiki/index.php?title=Raspi_EDLC_UPS)

[Lutz Lisseck]决定只用他的黑客包中的主电源开关来打开和关闭他的环境灯。他可以使用电池组构建一个传统的 UPS(毕竟只有 5V！)但决定更进一步。他拿起一对 50F 超级电容器。这样，他的 UPS 将比他的 Pi 持续更长时间！当主电源被切断时，电容储存的电量刚好足够 GPIO 注意到并告知 Pi，然后开始持续约 30 秒的关机序列。

虽然[Lutz]使用两个 2.7V 超级电容，但他提到使用升压转换器比串联更便宜，但他手头有电容，所以决定两个都用。

如果你需要它持续更长一点时间，你可以[做一个充电电池的…](http://hackaday.com/2013/11/17/battery-backup-for-raspi-keeps-your-data-safe/)