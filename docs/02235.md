# 树莓 Pi 四轴飞行器

> 原文：<https://hackaday.com/2012/12/01/raspberry-pi-quadcopter/>

[https://www.youtube.com/embed/TjXvzMdf8Nk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/TjXvzMdf8Nk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

这是迟早的事，但这并没有削弱[马修]的[树莓 Pi 驱动的四轴飞行器](http://www.botched.co.uk/picopters-maiden-flight/)的魅力。

[Matthew]的四轴飞行器与我们之前见过的所有其他飞行无人机相似，但有一个重要的区别——所有的处理，从读取陀螺仪到计算每个马达到底需要多少功率——都由一个树莓 Pi 处理。这项任务通常是微控制器的领域，因为这些计算需要实时进行。Matt 在他的 Pi 上运行的 Linux 发行版比简单的 AVR 或 ARM 微控制器有更多的开销，所以不能保证实时完成所有需要做的事情。通过一点巧妙的编程，[马修]设法确保所有必要的任务都得到及时处理。它仍然不是一个实时操作系统，但至少对于这个项目来说，它已经足够好了。

由于[马修]的四轴飞行器中的 Raspberry Pi 比微控制器强大得多，所以在飞行时有足够的顶部空间来 SSH 到该飞行器中。甚至可能有足够的处理能力将视频传输到网络服务器；老实说，我们迫不及待地想看看[马修]在未来会用他会飞的 Linux 电脑做什么。

你可以在 git 上查看【马修】的代码[，或者在他的 youtube](https://github.com/big5824/Picopter) 上观看一些飞行测试视频[。](http://www.youtube.com/user/big5824/)