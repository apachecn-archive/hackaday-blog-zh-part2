# 逆向工程点击剪辑

> 原文：<https://hackaday.com/2014/01/01/reverse-engineering-hitclips/>

![hitclipz](img/8a15ed6aef1d452c414fce5c8a5b984a.png)

在快速回顾了 Hackaday 的观众人口统计数据后，我们不得不说 90 年代末很奇怪。甚至连便携式音频播放器都十分怪异:MP3 播放器是存在的，但你通过电脑的并口下载你的歌曲(全部八首)。在帮助一个表亲搬家具时，[Ch00f]发现了大量有史以来最奇怪的音乐格式之一:HitClips，一种微小的塑料封装电路，可以存储 60 秒听起来很糟糕的单声道音频。是的，这是一个东西，但宠物石也是。由于没有 HitClips 播放器，[Ch00f]决定他将[对这些微小的歌曲进行逆向工程](http://ch00ftech.com/2013/12/31/reverse-engineering-a-hit-clip/)。

在拆开塑料外壳后，[Ch00f]发现了一个非常简单的电路:几个电阻、一个盖子和一个环氧树脂滴，后者封装了一个带有音乐数据的芯片。在夹子的背面，有八个用于连接播放器的衬垫。在一无所获的情况下，[Ch00f]开始四处摸索，发现将其中一个引脚接地会导致电路汲取 300uA 的电流约 60 秒，与记录的样本时间长度相同。

[Ch00f]最初认为 HitClip 将通过 SPI 或其他数字协议提供音频数据。他的发现更有趣:HitClip 上的两个引脚对应于 D 类放大器的推挽 fet。HitClip 上的音频是数字音频，但它经过编码，因此可以直接驱动模拟电路。如果你问我们，这是一个非常聪明的快乐餐玩具工程。

用逻辑分析仪转储这些数据后，[Ch00f]将所有值都转储到。WAV 文件。令人惊讶的是，那是音乐。对确定时间的过程进行了一点改进，得到了一个 60 秒的剪辑。)休息之后。

由于[Ch00f]不想花 40 美元在易贝上买一个老式的 HitClips 播放器，他对这些廉价的蹩脚音乐芯片的逆向工程已经到了极限。不过，他已经把他所有的文档都上传了，所以如果你想改进[Ch00f]的方法，那就试试吧。

[https://w.soundcloud.com/player/?url=http%3A%2F%2Fsoundcloud.com%2Fch00ftech%2Fpushpull&width=false&height=false&auto_play=false&hide_related=false&visual=false&show_comments=false&color=false&show_user=false&show_reposts=false](https://w.soundcloud.com/player/?url=http%3A%2F%2Fsoundcloud.com%2Fch00ftech%2Fpushpull&width=false&height=false&auto_play=false&hide_related=false&visual=false&show_comments=false&color=false&show_user=false&show_reposts=false)