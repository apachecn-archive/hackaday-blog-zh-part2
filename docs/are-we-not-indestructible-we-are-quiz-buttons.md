# 我们不是坚不可摧的吗？我们是测验按钮！

> 原文：<https://hackaday.com/2014/01/31/are-we-not-indestructible-we-are-quiz-buttons/>

我们希望这是面试中的一个新趋势，一些在[安东尼]工作的地方的人让他[做一些无线测试按钮](http://www.anthonyvh.com/2014/01/08/wireless-quiz-buttons/)。他非常认真地对待这项任务，使它们变得非常健壮和低功耗。

[Anthony]在按钮艺术方面很有经验，他为一个婚宴制作了[这个派对按钮](http://www.anthonyvh.com/2013/09/25/party-pushbutton)。他的测验按钮设计有点不同。每个按钮都有一个 Arduino Pro mini 和一个 nRF24L01 无线射频模块。在接收器端是一个 Arduino Pro micro 和另一个 RF 模块。连接的 PC 捕获串行数据并显示按下的按钮的 ID。它还显示了按下后续按钮的顺序以及它们之间经过的时间。

除了令人敬畏的激光切割 MDF Devo energy dome 按钮外壳之外，该产品真正值得注意的部分是传输 Arduinos 的极低功耗。[Anthony]设计它们进入睡眠模式，禁用所有板上电路，仅在中断时唤醒。他移除了电源 LED 和电压调节器，因为它们使用 2 节 AA 电池。电压调节器在睡眠模式下消耗的电流超过 25mA。由于这些模块，每个按钮的功耗小于 1μA，这比电池在其使用寿命期间的自放电功率还低。

[谢谢杰夫]