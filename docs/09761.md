# 黑客用平板扫描仪读取磁条卡

> 原文：<https://hackaday.com/2015/08/07/hacker-reads-magnetic-stripe-card-with-flatbed-scanner/>

【anfractuosus】一直在[读取磁条卡](https://www.anfractuosity.com/projects/optical-magnetic-stripe-reading/) …光学！

虽然黑客们通常是由[读取](http://hackaday.com/2009/08/19/quick-and-dirty-magnetic-card-reader/)和[写入](http://hackaday.com/2015/02/25/hacking-oklahoma-state-universitys-student-id-cards/)磁条卡，但这是我们第一次报道从磁条上光学成像和解码数据。[anfratuosus]使用了一种磁性显影剂，这种显影剂可以对磁条进行目视检查。显影剂使用悬浮在悬浮液中的微米大小的铁颗粒，这些颗粒被滴到条纹上。对粒子来说，磁条看起来像一系列排列的磁铁。长磁铁 [![stripe](img/bac13b6045db530d6d63c1a0949b9b82.png)](https://hackaday.com/wp-content/uploads/2015/08/stripe1.png) 代表 0，短磁铁代表 1。磁铁的方向随着每一位的变化而变化，就像右图一样。两极相遇的地方磁场最强。因此，铁粒子被吸引到条纹上的这些通量反转点，形成了一个可见的图案。下面有一个很棒的视频展示了这个过程。

虽然 magnetic developer 是为调试故障记录系统而设计的，但[anfratuosus]更进一步扫描“开发”的卡，并编写一个工具来解码图像和提取卡数据。[anfratuosus]没有提到任何特定的应用，但我们喜欢这种迂回的攻击方式！

[https://www.youtube.com/embed/2vaf1w101cg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/2vaf1w101cg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)