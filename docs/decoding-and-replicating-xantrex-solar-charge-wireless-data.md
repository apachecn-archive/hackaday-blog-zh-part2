# 解码和复制 Xantrex 太阳能充电数据

> 原文：<https://hackaday.com/2015/05/03/decoding-and-replicating-xantrex-solar-charge-wireless-data/>

这主要是一个解码数据的故事，但有一个美好的结局，包括将解码工作变成一个开源接收器。Xantrex solar charge controllers 监控大量关于太阳能电池板的数据，并通过 RJ25 传输，但您需要其附加硬件才能接收。[Eric Herbers]认为，如果数据正在传输，[足智多谋的黑客应该能够解码它](https://hackaday.io/project/5167-xantrex-c35c40c60-display)。他在黑客社区的朋友的帮助下做到了这一点。

我们在 Twitter 上询问人们在做什么，然后[Eric]发布了他的 scope 截图。接下来的对话帮助他找到了正确的方向，其他了解这个项目的人肯定会驱使他完成这个项目。解码并不完美，但足以解码和显示电压、电流和温度。[Eric]使用 Arduino Pro Mini 和最常见的黑色项目箱中的字符 LCD 构建了显示单元。