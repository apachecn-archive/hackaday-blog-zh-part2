# 我是 NXT 三点弯曲测试仪。请插入大梁。

> 原文：<https://hackaday.com/2013/12/29/i-am-nxt-3-point-bend-tester-please-insert-girder/>

视觉学习非常有帮助。用 NXT Mindstorms 制作的模型学习简直太棒了，正如[Rdsprm]用这个[乐高 NXT 三点弯曲测试仪](http://www.youtube.com/watch?v=_iFjY12M1fk)展示的那样，他建造这个测试仪是为了向新生介绍[弯曲挠度](http://en.wikipedia.org/wiki/Three_point_flexural_test)和材料特性。具体来说，它使用弹簧施加的力和梁的挠度来计算杨氏模量。[Rdsprm]在上面链接的 YouTube 视频的“关于”部分提供了详尽的解释，但 reddit 的评论绝对是一个增值。

[Rdsprm]从 Mindstorms 教育基础集( [9797](http://education.lego.com/en-us/lego-education-product-database/mindstorms/9797-lego-mindstorms-education-base-set) )和教育资源集( [9648](http://www.legoeducation.us/eng/product/lego_mindstorms_education_resource_set/2214) )构建了这个。每个参赛者都要经受 5 次电池测试，每次都应该产生相同的结果。前景中的电机设置梁的测试长度，第二个电机使用齿轮箱和链条拉下弹簧。

正如[Rdsprm]解释的那样，这种挠度测试方法是非传统的。通常，梁是增量加载的，在每个加载状态下测量挠度。这里，梁是连续加载的。垂直偏转是通过一个光传感器测量的，当光束通过时，光传感器读取光束上的条形码刻度。计算弹簧位置并用于确定施加的力。

[Rdsprm]分析了 GNU 倍频程的波动，并绘制了[光传感器读数](http://i.imgur.com/xy3O968.jpg)和[力-偏转](http://i.imgur.com/3fw0A3o.jpg)的图表。你的思维风暴不会让横梁弯曲？你可以把[改成这个 Ruzzle 播放器](http://hackaday.com/2013/02/19/lego-stylus-solves-ruzzle-tablet-game/)。

[https://www.youtube.com/embed/_iFjY12M1fk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/_iFjY12M1fk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [reddit](http://www.reddit.com/r/engineering/comments/1tn1uh/i_built_a_three_point_bend_test_out_of_lego_nxt/)