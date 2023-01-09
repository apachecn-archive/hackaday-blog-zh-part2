# 预算腕控遥控汽车是一个很好的接触

> 原文：<https://hackaday.com/2015/01/15/budget-wrist-controlled-rc-car-is-a-nice-touch/>

你的遥控汽车粗糙的按钮控制器是否让你觉得你像穴居人一样捣鼓电视遥控器按钮？我们也这么认为，但是[Noel]实际上已经做了大量的工作来解决这个问题。他[改造了他孩子的遥控器来控制手势](https://www.youtube.com/watch?v=K73akG-qWI0 "revamped his kids' rc controller for gesture control")。现在，他们的遥控车可以通过一个人的手腕运动的清晰，直观的控制来引导。

为了解决这个项目，[Noel]集成了一个陀螺仪和加速度计、一个 Arduino 和现有的遥控器。来自陀螺仪和加速度计限值的数据通过 Arduino 映射到按钮上，Arduino 解析原始数据并触发控制器的开关，现在直接连接到 Arduino 并通过电阻上拉。在他的[概述视频](https://www.youtube.com/watch?v=MP1wo0sJzMQ "overview video")中，【Noel】告诉我们，他已经将陀螺仪和加速度数据二进制化，以便在特定限制下触发，这一选择非常适合控制器的原始按钮控制。最后，整个装置干净地绑在一个 3D 打印的盒子上。还不错，总共 20 美元，还能快速到达目标。

[Noel]的定制手腕控制器在[许多其他独特控制器](http://hackaday.com/2013/06/20/building-custom-game-controllers-for-people-with-physical-disabilities/ "many other unique controllers")的货架上占据了一席之地，他的演示是一个利用现有开放硬件来定制我们的玩具以满足更多个人口味的绝佳例子。毕竟，硬件购物清单只是一个分线板、一个 Arduino 和几根跳线。当下一次僵尸末日来临的时候，我们可以很容易地看到一些像这样的实用组件进入我们的行李箱。至少，我们将能够制造一些手腕控制器，并派遣一些玩具车来迎接亡灵。

[https://www.youtube.com/embed/MP1wo0sJzMQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/MP1wo0sJzMQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)