# Nrf24l01+使用 3 个 ATtiny85 引脚

> 原文：<https://hackaday.com/2014/02/16/nrf24l01-using-3-attiny85-pins/>

[Ralph]对驱动他的 nrf24l01+收发器模块所需的 5 个控制引脚不满意，[所以他使用了这个只需要 3 个引脚的电路，使用了 ATtiny85](http://nerdralph.blogspot.ca/2014/01/nrf24l01-control-with-3-attiny85-pins.html) 。

其中一个关键组件是从时钟(SCK)线有效地驱动芯片选择(CSN)线。nrf24l01+需要 CSN 线在通信开始时从高电平转换到低电平。[Ralph]将 SCK 线放在二极管后面，将一个电容器与 CSN 线并联，并修改了 [arduino-nrf24l01 库](https://github.com/stanleyseow/arduino-nrf24l01)以编码时钟线的额外延迟。这使得 CSN 线可以由 SCK 线驱动。传输过程中的后续线路转换发生得太快，无法对电容充电，导致 CSN 线路处于低电平状态。

在将芯片使能线连接到高电平并将红色 LED 两端的 5V 电源线降至 1.9-3.6V 后，[Ralph]有一个 ATtiny85 控制 nrf24l01+模块。

虽然看似简单，但这是一个非常酷的黑客技术，它在 ATtiny85 上开辟了几条新的线路。