# 使用 Arduino 读取 2.4GHz 发射机

> 原文：<https://hackaday.com/2014/05/10/reading-2-4ghz-transmitters-with-an-arduino/>

市面上有很多便宜的四轴飞行器套件，出售时带有发射器和电池，售价约为 50 美元。这些微型四轴飞行器中比较受欢迎的一个是 V2X2 系列。不幸的是，它们与任何其他无线电协议都不兼容，但[Alexandre]已经成功使用他的 V202 quad [中包含的发射器向 Arduino](http://www.wavecruncher.net/~execuc/projects/pv202_receiver/) 发送数据。

像大多数四轴发射器一样，与[Alexandre]的 V202 一起提供的发射器工作在 2.4GHz。监听该频段需要一点硬件，在这种情况下，是一个北欧半导体 nRF24L01p。附在这个芯片上的是一个常规的‘ol Arduino[运行一点代码](https://github.com/execuc/v202-receiver)，其中包括【Alexandre】的 V202 库。

现在，构建可以检测 quad 是否绑定，并读取油门、偏航、俯仰和滚动的当前位置，以及所有相关的微调。这只是[Alexandre]项目的开始，但他的最终目标是基于代码建造一个 Arduino 机器人，配有 RC 伺服系统。对于一个当微四边形最终破裂时将完全无用的发射器来说，这并不坏。

[https://www.youtube.com/embed/dus7GxoRIEk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/dus7GxoRIEk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)