# P.u.l.s.e 停车灯

> 原文：<https://hackaday.com/2014/05/08/the-p-u-l-s-e-parking-light/>

[Anool]的哥哥喜欢他的摩托车，当他看到刹车灯的“呼吸 LED”模块时，他不得不拥有一个。[被赋予创造一个非常酷的模型的任务，](http://wyolum.com/p-u-l-s-e-fader-control-for-motorcycle-parking-lamp/) [Anool]想出了 p.u.l.s.e，一个极小的 LED 控制器，有点像平克·弗洛伊德和第二或第三大 CD 包装。

该电路是一个稍微受苹果启发的停车灯模块，当自行车上的中性检测线高时，灯保持完全点亮，当中性检测线低时，LED 以“呼吸”模式缓慢脉冲。这么简单的事情不需要太多逻辑，所以[Anool]转向 ATtiny45 和 Arduino IDE 来实现他的目标。

[Anool]在 KiCAD 中创建了一个电路，可以插入他哥哥自行车的灯座。一簇 led 取代了停车灯内的 T10 灯，少量代码负责逻辑和呼吸效果。这是一个伟大的 mod，令人惊讶的小尺寸的电路板使他成为我们见过的最小的 Arduino 的竞争者。

下面是行动中的光的视频。

[https://www.youtube.com/embed/5qYFoy7ZsJ4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/5qYFoy7ZsJ4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/wrf8d8C7XTc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wrf8d8C7XTc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)