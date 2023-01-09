# 克隆 Tektronix 应用模块

> 原文：<https://hackaday.com/2014/07/28/cloning-tektronix-application-modules/>

Tektronix 的 MSO2000 系列示波器是很好的工具，加上一些“应用模块”，可以完成一些非常有趣的任务:解码串行协议、嵌入式协议，如和 SPI，以及汽车协议，如 can 和 LIN。在测试他的 MSO2012B 时，[jm]非常喜欢 I2C 解码器的(限时)演示，但认为它不值得该应用模块 500 美元的售价。没关系，因为它只是一个廉价的 24c08 EEPROM 上的一些数据，并带有一点 PCB 设计`<<removed because of dmca takedown>>`

Tektronix 销售的应用模块只是一个加载了`<<removed because of dmca takedown>>`的小 EEPROM。通过将该值写入 0.25 美元的 EEPROM，[jm]可以使能两种应用。唯一的问题是让他的示波器读取 EEPROM:这个问题很容易用定制板解决。

电路板[jm]设计了`<<removed because of dmca takedown>>`，唯一需要的附加元件是一个 EEPROM，一组用于读取 SIM 卡的触点，以及一点点粘在电路板背面用于适当间隔的塑料。

**更新:**了解促使本帖修改的 DMCA 撤下通知:http://hack aday . com/2014/08/05/hardware-security-and-a-dmca-take down-Notice/