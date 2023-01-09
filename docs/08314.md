# 自动抄表馈线保持米女佣在海湾

> 原文：<https://hackaday.com/2015/02/14/auto-meter-reader-feeder-keeps-meter-maids-at-bay/>

把你的车放在任何地方几乎都要付出代价；而且，如果你的回报已经过期，很有可能你会付出比预期更高的价格。停车计时器是一种奇妙的装置，可以告诉当局你还剩多少时间可以使用。[Zack]认为迟到 5 分钟——甚至 10 分钟——是一个支付罚款的荒谬理由，所以他开发了一个工具，当当局过于接近时，它会[在仪表中预装一些额外的硬币](https://www.youtube.com/watch?v=4erjjDiA5lU)。

执法检测系统整合了许多我们非常熟悉的工具和技术:3D 打印、Arduino、光敏电阻和接近(PIR)传感器。在代码级别，[Zack]用滚动平均值过滤他的模拟光敏电阻，以获得白天和晚上都可以触发的干净信号。触发器？两种可能。PIR 传感器检测好奇的执法人员，而过滤光敏电阻检测周期性旋转的警笛灯。这两个事件都会给螺线管通电，使一些额外的硬币通过滑道落入投币口。

对于一个众所周知的组件集合，[扎克]可以把他的装置装进一个 Altoids 罐，然后收工。并非如此。作为一名交互设计师，外观可以决定体验的成败。出于这个原因，他选择了蒸汽朋克风格的抱脸设计。此外，为了实现一系列设备的兼容性，[Zack]的 CAD 模型是根据他在城市荒野拍摄的图像对各种仪表配置文件进行调整的结果。结果呢？与一系列仪表兼容的干净、真实的设备。

对于目光敏锐的观察者来说，[扎克]的第一个视频发布于 2011 年，但他的作品后来在 2015 年[有形、嵌入和具体化会议](http://hackaday.com/?s=tei)的一次演示中重新浮出水面，他的前设计导师[埃里克·保罗斯]急于展示[扎克]的作品。为了更深入地了解即将出版的第二版，请前往【扎克的】[图片订阅](https://drive.google.com/folderview?id=0B1s_fJPcZmzXU3JaZ1NjSnpHZ2c&usp=sharing)。

[https://www.youtube.com/embed/4erjjDiA5lU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/4erjjDiA5lU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)