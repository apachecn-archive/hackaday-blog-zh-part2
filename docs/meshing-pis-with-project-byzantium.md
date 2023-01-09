# 将 Pis 与拜占庭项目相结合

> 原文：<https://hackaday.com/2015/04/28/meshing-pis-with-project-byzantium/>

如果互联网服务提供商倒闭，我们如何让我们的设备进行通信？拜占庭项目旨在创建一个“僵尸末日专用无线网状网络”这是一个实时的 Linux 发行版，使加入一个安全的网状网络变得容易。

[B1 TSH 1 after]已经组装了一套硬件，用于在紧急情况下在 Pis 上运行[拜占庭](http://b1tsh1fter.blogspot.ca/2015/04/scalable-mesh-network-wifi-1.html)。一个 Raspberry Pi 2 充当网状节点，使用强大的 USB WiFi 适配器进行联网。提供备用电源选项，包括太阳能充电器和基于超级电容器的解决方案。

Pi 运行标准的 Raspbian 安装，但是使用来自 [ByzPi 库](https://github.com/Byzantium/ByzPi)的包。这提供了一个在 Pi 上启动并运行 Byzantium 节点的脚本。在后台， [OLSR](http://www.olsr.org/mediawiki/index.php/Main_Page) 用于通过网状网络路由数据包，使节点可以不依赖单一链路进行通信。

这个项目还有很长的路要走，但是基于 Raspberry Pi 的设置使得建立和运行广域网变得便宜和容易，而不依赖于单一的权威。