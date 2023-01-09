# PiAware，树莓 Pi 上的自动航班跟踪

> 原文：<https://hackaday.com/2014/08/25/piaware-automated-airliner-tracking-on-the-raspberry-pi/>

![FlightAware](img/c74eed5d6be3498dfc32839024a8be89.png)

对于那些极客航空迷来说，FlightAware 是一个追踪目前飞行中的几乎每一架客机和大多数私人飞机的网站。FlightAware 的人员在世界各地几千名志愿者的帮助下汇编所有信息，这些志愿者有一点硬件来监听 ADS-B 传输，并将它们转发到 FlightAware 的服务器。现在你可以用一个树莓派来做这件事，作为一个不错的小奖励，FlightAware 向任何人免费赠送企业账户。

监听 ADS-B 转发器是 Raspberry Pis 已经做了一段时间的事情，但是对头顶飞过的各种飞机的高度、速度、航向和注册号做任何有用的事情几乎是 FlightAware 存在的唯一理由，也是他们为 Pi 开发易于使用的软件包的原因。

设置一切需要[在 Pi](http://www.satsignal.eu/raspberry-pi/dump1090.html) 上运行 dump1090，唯一需要的硬件是 RTL-SDR USB 电视调谐器、GPS 模块和 1090 MHz 天线。从那里，只需将所有数据发送到 FlightAware，你就可以获得一个免费的企业账户。对于航空爱好者来说，这是一笔不错的交易。