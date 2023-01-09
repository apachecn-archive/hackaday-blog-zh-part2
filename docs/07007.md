# ESP8266 开发的现状

> 原文：<https://hackaday.com/2014/09/06/the-current-state-of-esp8266-development/>

几周前，我们听说了一种非常酷的新芯片。它被称为 ESP8266 ，是一个 WiFi 模块，允许您将任何项目连接到 802.11 b/g/n 网络。也要 5 美元。是的，当这个芯片被宣布的时候，有很多欢乐。

自从我们了解到 ESP8266 之后，已经做了大量的工作来翻译中文数据手册，弄清楚如何对 SOC 进行编程，并对该模块与 Arduino 配合使用做了一些初步尝试。请记住，现在很少有人手头有这些模块之一，所以所有这些信息都是完全未经测试的。这是我们目前掌握的情况:

在 Hackaday 项目中，[【bafeigum】一直在研究这个模块的能力。大部分的评论都是关于模块的 AT 命令集和计算当某些命令被调用时实际返回的内容的](https://hackaday.io/project/2879-ESP8266-WiFi-Module-Library)[。](https://hackaday.io/project/2879/log/9300-more-at-command-information-found)

[ESP8266 社区论坛](http://www.esp8266.com/search.php?search_id=active_topics)成立大约一周了，但是已经有了大量的信息。大多数努力似乎都集中在[让 GCC 对这个芯片](http://www.esp8266.com/viewtopic.php?f=9&t=19&sid=2bcffde786cfebbd3a1cfa422e7ffdbb)进行编程，这将使 ESP8266 成为任何需要 WiFi 和一点处理能力的单一解决方案芯片。每个人(包括伟大的[Sprite_TM])目前都遇到了障碍，所以如果您对 GCC 和 Xtensa 微控制器有丰富的经验，请查看该线程。如果做不到这一点，我们将不得不等待来自 Tensilica 的人，这个芯片背后的公司，插话并帮助每个人弄清楚这个东西实际上是如何工作的。

外面的 Arduino-heads 会过得更轻松。[已经有一个将 ESP8266](https://www.zybuluo.com/kfihihc/note/31135) 用作串行 WiFi 模块的教程。请注意，ESP 在 3.3 伏电压下运行，因此将该模块连接到 5V 引脚意味着您将损失 5 美元和几周的运输时间。

这是在很短的时间内取得的令人难以置信的发展，更令人瞩目的是*还没有人拥有这些 WiFi 模块*。当这些模块到达世界各地的工作台时，我们预计 Hackaday tip line 将被非常小且有点电池友好的 WiFi 版本所淹没。