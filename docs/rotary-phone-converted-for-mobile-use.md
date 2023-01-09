# 转换为移动使用的旋转式电话

> 原文：<https://hackaday.com/2015/05/31/rotary-phone-converted-for-mobile-use/>

作为一个社会，我们正在远离固定电话，而移动设备变得越来越普遍。人们只有一部手机而完全不用有线家庭电话的情况并不少见。虽然这一举动可能是为了方便，但这两种手机有一个不同之处，这让[斯塔夫罗斯]很不舒服。他是一个愤怒的电话交谈者，并错过了摔下电话听筒的能力。现在[Stavros]可以只拥有一部有线家庭电话，但他想要一个手机 slams 的移动选项，所以他想出了一个名为[I rotary](http://www.stavros.io/posts/irotary-saga/)的项目。这是一个老式的旋转式电话，由电池供电，使用手机网络打电话。

该项目的核心是一个 Arduino。Arduino 是一个很好的选择，因为它可以轻松解码手机的旋转拨号脉冲。Arduino 代码将所有单独拨打的号码组合成一个电话号码。草图设置为在读取第 10 个数字后，使用现成的 GSM 屏蔽和相关库拨打电话。

因为电池是移动电话所必需的，所以电池和充电电路一起被安装在外壳里。[Stavros]没有做过任何长期的耐力研究，但他一次开几个小时的电话，没有任何问题。所以，现在他可以高枕无忧了，因为他知道，无论他身在何处，愤怒的障碍永远不会远离他。因为他是一个好人，他为任何想做类似东西的人提供了源代码。

[https://www.youtube.com/embed/fSkdWQswpc8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fSkdWQswpc8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)