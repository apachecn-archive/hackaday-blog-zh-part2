# 在高压键盘上播放音乐

> 原文：<https://hackaday.com/2014/11/17/play-music-on-a-high-voltage-keyboard/>

[Matt]在一家霓虹灯电源公司工作。当一个供应商的失误给他留下了相当多有缺陷的高压变压器时，他无法让自己把它们扔进垃圾箱。[Matt]能够很好地修复变压器，使其正常工作，一个高压键盘的想法开始酝酿。不幸的是，最初的变形金刚无法胜任创造音乐弧线的任务。从那时起，这个项目就有了自己的生命。马特抓起一些功率更高的变压器，开始建造。

键盘有 25 个键，每个键都连接到一个单独的高压电路，有自己的火花隙。高压电路基于 [IR2153D 自振荡半桥驱动器。](http://www.irf.com/product-info/datasheets/data/ir2153.pdf) (PDF 链接)。2153D 由一个很好的老式 555 定时器芯片调制。伙计们，这个设计里没有微型！IR2153D 的输出切换一对驱动反激式变压器的 N 沟道 MOSFETS。

[Matt]制作了他的电路的 25 个副本，并在单独的 PCB 上构建它们。他把所有的东西都组装在一块形状大致像三角钢琴的木板上。最终的项目看起来很棒——尽管[马特]不可否认没有音乐才能，所以我们还不能听到 AC/DC 从那些火花隙中飞出。

如果你确实想听斯帕克斯演奏音乐，那就去看看我们在 2013 年纽约 MakerFaire 上看到的 [OneTesla 项目](http://hackaday.com/2013/09/24/onetesla-electrifies-maker-faire-ny-2013/)。

[https://player.vimeo.com/video/111985661](https://player.vimeo.com/video/111985661)