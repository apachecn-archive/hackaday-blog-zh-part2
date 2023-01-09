# 亚马逊 Echo 订购 Roku 大约

> 原文：<https://hackaday.com/2015/08/01/amazon-echo-orders-the-roku-about/>

你可以将 Roku 媒体播放器添加到可以由亚马逊 Echo 及其内置人工智能 Alexa 指挥的设备列表中。[Julian Hartline]已经想出如何使用亚马逊的声控回声设备和 Roku 媒体播放器。他通过使用 [Alexa 技能工具包](https://developer.amazon.com/appsandservices/solutions/alexa/alexa-skills-kit)来实现这一点，该 SDK 为程序员提供了进入设备功能的界面。这允许你给 Alexa 和处理语音命令的 [AWS Lambda 云服务](http://aws.amazon.com/lambda/)添加功能(亚马逊称之为 Alexa 的技能)。

然而，他没有让云服务直接与 Roku 对话，而是决定让一个本地 node.js 服务器充当中介。Alexa 将语音命令发送给 AWS Lambda 服务，后者对其进行处理，然后将命令发送给 node.js 服务，后者最终将命令发送给 Roku。有效果，但是反应好像有点慢:休息后看视频。在所示的例子中，Alexa 实际上让 Roku 启动了网飞，并为请求的节目输入了搜索字符串。相当光滑！

[Julian]使用 node.js 中介有两个原因。一是可以更容易地向服务中添加更多设备，因为可以更容易地向 node.js 服务器添加对新设备的支持，比如他已经添加的 IR blaster 支持。第二，他说 Alexa 本身不能直接向新设备发送命令:它存在于你的本地网络中，但不能向它没有内置支持的设备发送命令。“不幸的是，这个问题在目前的情况下有点局限”[Julian]告诉我们。“我假设 WeMo 功能是使用 Echo 与本地网络的连接来完成的。我希望(并期待)有一天第三方开发者能够获得这一功能。”我们也希望如此。他提到的 WeMo 功能[已经被黑客攻击](http://hackaday.com/2015/07/16/how-to-make-amazon-echo-control-fake-wemo-devices/)作为一种额外的方式来连接到封闭的 Echo 系统。

[https://www.youtube.com/embed/fcn1gUd7Tbw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fcn1gUd7Tbw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)