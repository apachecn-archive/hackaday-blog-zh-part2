# 将单极步进器更改为双极

> 原文：<https://hackaday.com/2014/07/29/changing-unipolar-steppers-to-bipolar/>

如果你是一个优秀的小黑客，并且像你应该做的那样拆旧打印机，你可能遇到过不止几个步进电机。这些电机有多种类型，从 3D 打印机构建中的四线交易到五线或六线电机。单极电机——四线以上的电机——更容易控制，但在产生扭矩方面受到严重限制。幸运的是，[您可以使用任何单极电机作为更高效的双极电机](http://www.jangeox.be/2013/10/change-unipolar-28byj-48-to-bipolar.html),只需对 xacto 刀进行简单修改。

单极电机中的额外电线是每个线圈的抽头。简单地忽略这些导线并独立使用两个线圈使电机更有效地产生扭矩。

[Jangeox]做了一个小实验，采用单极电机，切断线圈抽头的走线，测量前后扭矩。结果令人印象深刻:作为单极电机，电机的扭矩约为 380 gcm。在双极模式下，同样的电机有 800 gcm 的扭矩。你可以看看下面的视频。

[https://www.youtube.com/embed/jHLyJbNgcDo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/jHLyJbNgcDo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)