# 黑掉 Oculus Rift:Oculight

> 原文：<https://hackaday.com/2013/04/11/hacking-the-oculus-rift-the-oculight/>

[https://www.youtube.com/embed/r8FSuxA-cp4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/r8FSuxA-cp4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

我们的 [Oculus Rift](http://hackaday.com/2012/08/17/were-getting-an-oculus-rift-dev-kit/) 终于邮寄到了。除了说它令人惊奇之外，我不会告诉你我对这个项目本身的想法。有大量的视频可供选择，显示人们的想法和反应， [Ifixit 也有他们通常的详细拆卸](http://www.ifixit.com/Teardown/Oculus+Rift+Teardown/13682/1)。

我决定首先解决的是水平周边视觉灯。眼睛的形状意味着你感觉像戴着一个潜水面具。在两侧的远边缘有大的黑色边框。看起来一个简单的模式是添加一些 RGB LEDs 并运行一个简单的流光溢彩克隆。

我下载了 Adalight 代码,插上了我放在身边的一个 RGB LED 灯。裂缝的四个角落有一些网状区域，让空气在那里流动。我利用了这一点，所以我甚至不需要切开裂缝…到目前为止。我只是简单地把带子绑在裂缝上，让合适的发光二极管穿过小孔。

结果还不错。由于 led 在你的外围视觉中比屏幕边缘更靠后，看起来周围的一点光可能只是“漏”进了耳机。给人的感觉是看到了远在屏幕边缘之外的东西。一个更好的安装，让灯一直照在左右两边，而不仅仅是角落，可能会产生更好的效果。