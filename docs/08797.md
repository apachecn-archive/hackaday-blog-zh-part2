# 用你的家用植物玩机器人手鼓

> 原文：<https://hackaday.com/2015/04/16/play-robotic-bongos-using-your-household-plants/>

[Kirk Kaiser]不怕承认他的最新项目有点奇怪，是一套由工厂控制的机器人手鼓。我们一点也不觉得奇怪。这是我们喜欢看到的事情。他的项目起源于一个月前，当时他在[纽约电阻器](http://hackaday.com/2014/06/13/nyc-resistor-interactive-show-2014/)上了一堂关于用机器人乐器创作音乐的课。[ [柯克](http://hackaday.com/2013/03/20/measuring-meditation-with-a-heart-rate/)受启发制作了自己的盘子，他将邻居的旧木制盘子架用作螺线管的支架，当螺线管被触发时，就会敲击几个塑料牛铃或小鼓。

Raspberry Pi 最初用于将螺线管与计算机或 MIDI 键盘连接起来，但在油炸后，他用一个 Teensy LC 代替，并且从未回头。利用 Teensy 的 MIDI 特性，[Kirk]编写了一个特定的音符来触发每个螺线管。当他意识到 Teensy 也有电容式触摸传感器时，他决定让他的植物以一种 MaKey MaKey 的方式享受乐趣。每株植物都通过绞合线连接到青少年的触针上；另一端剥去，盖上铜带，放入土中。当植物的电容超过阈值时，相应的 MIDI 音符和螺线管就会被触发。[Kirk]很快发现[硬编码阈值](https://github.com/burningion/robotBongos)不是最好的主意。寻找大的变化是一个更好的方法，因为当植物的土壤变干时，电容会受到显著影响。当[柯克]退后一步欣赏他的作品时，他意识到少了一样东西——灯光！他连接了一个 Arduino，它有一个 [DMX 盾](http://shop.trinculosattic.com/products/the-guildenstern-arduino-dmx-shield)和一些只要植物被触摸就会发光的 led。

我们确实觉得对使用这种植物学技术感兴趣的任何人都有一个免责声明:带刺的品种是不明智的，除非你想恶作剧，让仙人掌成为关掉手鼓的唯一方式！

[https://www.youtube.com/embed/furZK3c88d8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/furZK3c88d8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)