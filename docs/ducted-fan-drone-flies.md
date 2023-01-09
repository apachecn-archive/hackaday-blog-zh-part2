# 涵道风扇无人机飞行

> 原文：<https://hackaday.com/2015/07/04/ducted-fan-drone-flies/>

不久前，我们写了[阿明·斯特罗贝尔]正在研究的涵道风扇、单旋翼、垂直起降无人机。那时它还没有完全完工，还没有起飞。他发布了一个更新，从它的外观来看，他已经取得了大量的进展，包括成功起飞和着陆的第一次飞行。

这次成功的飞行不是巧合。调整任何一种直升机都是一件棘手的事情。在测试过程中手动操作它们可能会非常危险。因此，他用木头、一些 3D 打印零件和轴承建造了两个不同的试验台。一个让他安装无人机并调整其俯仰(和滚动)，而另一个让他调整偏航参数。就像他们在风洞试验中所做的一样，他在空气框架的不同点上固定了一些短的纱线来检查湍流。这样做也让他对如何在下一次迭代中改进 3D 打印空气框架有了一些了解。他在两个测试台上重复了这些测试，来来回回以确保调整参数不会相互干扰。他还改装了起落架，以提高起飞和着陆时的稳定性，防止倾翻。[阿明]正在使用 [PixHawk PX4](https://pixhawk.org/choice) 进行飞行控制，使用 BeagleBone Black 进行高级功能和控制。

一旦第一次飞行表明无人机可以做稳定的飞行，他就附上一个 Go-Pro，并在随后的飞行中录制了一些不错的视频。接下来的步骤是微调飞行控制参数，以确保稳定的悬停与位置保持和航路点跟踪。他也可以 3D 打印一个改进的空气框架。关于建造的细节，请查看我们之前关于[涵道风扇无人机](https://hackaday.com/2015/05/30/ducted-fan-drone-uses-1-rotor-for-vtol/)的博文。看看下面的两个视频——一个展示了无人机的首次飞行，另一个是关于用于调整的试验台。

[https://www.youtube.com/embed/bHN5H3jyw-o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bHN5H3jyw-o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/wo-AJtD5CRs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/wo-AJtD5CRs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)