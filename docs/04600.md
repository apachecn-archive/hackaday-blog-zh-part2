# 后姿势视频游戏控制器

> 原文：<https://hackaday.com/2013/11/19/posterior-posture-videogame-controller/>

通常我们会看到一些疯狂的科学项目来自本·克拉斯诺的实验室。本周[Ben]稍微改变了一下方式，[将他的 Xbox 控制器与他的浴室体重秤](http://www.youtube.com/watch?v=vfqtKJAnJHg)连接起来，作为一个姿势控制输入设备。在我们试图解释之前，你可能需要一点时间来思考这个问题。这意味着你坐在浴室磅秤上，当你向前倾斜时，你的游戏角色向前移动，向后倾斜，你的角色向后倾斜，从一边到另一边进行左右扫射。

现代数字浴室秤有四个压力点传感器，每个角一个，由中央控制器读取并求和，以生成秤上物体设置的重量。为了将秤用作控制器输入,[Ben]移除了中央秤控制器，并创建了两个放大惠斯通电桥差分电路，称重传感器之间的每个对角线轴各有一个。在添加一个偏移电位计以将静止点固定在 0.8 伏后，放大的差分电压信号被直接馈送到 Xbox 控制器的拇指棒输入端以进行游戏控制。

此外，为了给他的新游戏控制器增加旋转功能，他黑了一个旧的球型鼠标，并添加了一点橡胶管，用于接触和跟踪一个懒惰的苏珊浅盘的底部。秤放在转盘上，允许你的躯干部分旋转，以控制游戏的旋转。然而，[本]仍然需要一个普通的鼠标与游戏接口，以实现完整的 360°旋转控制。

休息之后还有更多，加上构建和演示视频。

[Ben]如此努力的原因是为了拥有一个免提游戏控制设备，这可能对未来的虚拟现实游戏有用。我们也可以看到这种设备被用来帮助一些身体残疾的人。如果[Ben]想更进一步，将[语音控制添加到他的 Xbox 控制器](http://hackaday.com/2008/02/01/voice-controlled-game-controller/)中，我们已经有了一个参考项目可供阅读。

[https://www.youtube.com/embed/vfqtKJAnJHg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vfqtKJAnJHg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)