# 自拍机器人会帮你拍下最好的照片

> 原文：<https://hackaday.com/2014/12/25/selfie-bots-will-take-your-best-shots-for-you/>

布鲁斯·兰德教授在康奈尔大学教授微控制器课程，今年的主题似乎是自拍机器人。

首先是(韩，毕涵和川)对技术的巧妙组合。拿一部 iPhone，三个麦克风，一个微控制器会怎么样？自拍技术的终极设备，这就是——拍手！iPhone 安装在几个伺服电机上，这使得机器人可以将相机指向，你猜对了，鼓掌声。第二次拍手时，手机会给你拍照。可爱。

下一个有点复杂的是面部识别自拍机器人。当你的手臂不够长时，这个小机器人可以通过编程来跟踪人脸，并为你和你的朋友拍照。不仅如此，你可以设置各种参数，这样你就可以得到完美的图片。它使用 OpenCV 来处理原始数据，并向 ATmega1284 输出命令，atmega 1284 控制指导相机的伺服电机。这个项目是由康奈尔大学的两个四年级学生[迈克尔和詹妮弗]完成的。

[https://www.youtube.com/embed/erwi-TFy5Dk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/erwi-TFy5Dk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/QSPoOkb2TXs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/QSPoOkb2TXs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

虽然这些机器人似乎喜欢给人类拍照，但它们可能还没有发现像这个机器人一样的感知能力，这个机器人的虚荣心是无限的——只给自己和自己拍照。