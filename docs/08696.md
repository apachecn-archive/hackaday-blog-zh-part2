# 非无限但任意大量的视频馈送

> 原文：<https://hackaday.com/2015/04/06/non-infinite-but-arbitrarily-large-number-of-video-feeds/>

当你需要监控什么的时候，拿一个 USB 摄像头是很常见的。它们现在又快又简单，大多数在几乎所有现代操作系统上都是即插即用的，而且很便宜。但是，如果您需要监控的东西不止这些，会发生什么情况呢？这通常意味着大量的相机和额外昂贵的硬件来支持所需的强大软件，但[moritz simon geist]和他的团队的 Madcam 软件现在可以廉价而简单地做同样的事情。

在该小组决定使用 PCI 来处理视频馈送之前，考虑了许多方法。显然，只使用 USB 会导致瓶颈，但他们也发现以太网也有很高的延迟。他们还尝试混合来自 Raspberry Pis 的视频，但也没有取得多大成功。他们的计算机是一个非常标准的 AMD，有 4 GB 的内存，运行 Xubuntu，所以只要你有所需的 PCI 插槽，你就可以用这个软件做很多事情。

起初，我们对 500 美元左右的价格标签嗤之以鼻(包括运行该软件的计算机)，但显然，你在一个商业系统上的花费是无限的，所以这实际上是相当大的成本降低。很可能你已经有了一台台式电脑，一旦你从他们的 Github 仓库中获得了软件，你就差不多上路了。到目前为止，创作者已经用 10 个摄像头测试了该软件，但它可以扩展到处理更多的摄像头。如果你能以某种方式整合来自广播源的视频源，那就更酷了！

[https://www.youtube.com/embed/nk4oQDKUXEw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/nk4oQDKUXEw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)