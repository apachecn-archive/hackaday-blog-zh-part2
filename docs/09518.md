# 无创智能电表

> 原文：<https://hackaday.com/2015/07/11/non-invasive-smart-electricity-meter/>

有很多方法可以测量家中的能源使用量，但大多数都涉及到处理电源电压。不仅如此，有时它们需要在电源电压通过断路器面板或保险丝盒之前处理电源电压，这意味着如果你犯了一个错误，可能会发生很多糟糕的事情。[尤纳斯]一直在研究这个问题，并提出了一种[非侵入性的、更安全的方法来监控电力消耗](http://www.hackster.io/yleguesse/spark-non-invasive-smart-electricity-meter)，而不必直接在带电的电线上工作。

请注意，如果没有经过适当的培训，你仍然不应该在电源电压上工作，但是如果你有所需的专业知识，那么安装应该非常简单。该项目基于 Spark 核心，使用钳形电流传感器来测量能源使用。传感器缠绕在电源电缆上，这意味着你不必断开任何东西来连接它们。后端运行在一个 [LAMP 服务器](https://en.m.wikipedia.org/wiki/LAMP_(software_bundle))上，如果你有的话，它可能是一个 Raspberry Pi。[Yonas]偏好在托管服务器上运行它。

这方面的所有源代码都是可用的，假设你能接触到电流传感器，这可能是开始监控你在房子里的能源使用的一个很好的方法。请务必观看下面的视频，了解该设备的操作演示。当然，如果你有一条输气管道[，你也需要这个能源监控装置](http://hackaday.com/2015/06/30/disassembled-mouse-keeps-track-of-gas-meter/)。

[https://www.youtube.com/embed/myl4O06VrTQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/myl4O06VrTQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)