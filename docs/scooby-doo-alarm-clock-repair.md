# 史酷比闹钟修理

> 原文：<https://hackaday.com/2014/01/13/scooby-doo-alarm-clock-repair/>

[![Scooby-Doo_alarm_clock_repair.Still001](img/a5d4b5659ab9d0599d1504300684c358.png)](http://hackaday.com/wp-content/uploads/2014/01/scooby-doo_alarm_clock_repair-still001.jpg)

这与其说是修复，不如说是破解，这也是我展示我的[史酷比闹钟修复版](http://www.toddfun.com/2014/01/12/scooby-doo-alarm-clock-repair/)的一个好理由。我开始试图简单地修复一些损坏的硬件安装，这些硬件安装将显示屏和按钮机制固定在闹钟内，看起来像史酷比-杜神秘货车。在测试过程中，我注意到显示器非常暗，这表明存在不寻常的电流负载或其他故障，而且警报不起作用。

该报警器最酷的功能之一是，当报警器被激活时，它会发出汽车喇叭声。不幸的是，产生鸣笛声的板载芯片内部短路，导致一些晶体管过热和显示器变暗。不可能恢复定制芯片的功能，但幸运的是，LM8560 时钟芯片的数据表显示，它可以直接向扬声器输出标准的报警蜂鸣声。这要求 PCB 和一些电路采用不同的配置。

最后，时钟的当前负载下降到正常参数，显示器再次变亮，闹钟使用来自 LM8560 时钟芯片的标准哔哔声报警。令人难过的是，闹钟的凉爽因素无法通过鸣笛的汽车声音警报恢复，但我的儿子很高兴他最喜欢的史酷比闹钟再次发挥作用。

电路修改可能不是最聪明或最好的解决方案，所以如果你有其他建议，请在下面的评论中留下。休息后可以观看电路评估和维修修改的视频。

[https://www.youtube.com/embed/azaWPkFdKBo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/azaWPkFdKBo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)