# 用 LLVM 破解你的 C++

> 原文：<https://hackaday.com/2015/08/05/hack-your-c-with-llvm/>

你有没有想过分析或变异一些 C 或 C++代码？您可以使用正则表达式进行一些简单的模式匹配，但是总会有这样或那样的特例打破您的逻辑。为了做好这件事，你需要开发一个完整的解析器，也许使用正式的语法和像 Yacc 这样的工具。不过，这是一项很大的工作，仅仅是将所有的 floats 都改为 doubles。

[Adrian Sampson]写了一篇博客文章，让你从对编译器不感兴趣的状态转变为兴奋地使用 LLVM 做伟大的工作的状态。LLVM——低级虚拟机编译器基础设施——为许多语言提供了工具，包括 C 和 C++的 CLANG。[Adrian]指出了 LLVM 和其他用于类似目的的编译器和工具之间的一些关键区别:

*   LLVM 使用人类可读的一致的中间表示
*   它是高度模块化的
*   它既是高度可黑客化的，又是工业级的、得到良好支持的编译器

他指出，编译器工具不仅仅用于编译。您可以使用它们来分析源代码，构建模拟器，并为安全性或测试注入代码，等等(说到安全性测试，请在休息后查看使用 LLVM 来分析视频中的二进制文件的安全性问题)。LLVM 的高度可攻击性是由于它的模块化本质。默认情况下，前端将 C 或 C++代码分解成中间表示。然后，多次传递可以在将表示传递给下一次传递之前对其进行修改。最后一遍为目标处理器进行实际的代码生成。

添加通行证是相当容易的，而且[Adrian]甚至提供了一个模板和一个例子。很自然，您可以使用 pass 来进行某种特殊的或实验性的优化。但是除了代码优化之外，您还可以使用 pass 来分析或修改代码。

我们最近讨论了围绕定制 CPU 构建基础设施的[困难。提到了 LLVM，而且[Adrian 的]模板和示例将是创建定制 C 编译器的一个很好的开端。CLANG 甚至可以为](http://hackaday.com/2015/07/31/build-your-own-cpu-thats-the-easy-part/) [Arduino](http://hackaday.com/2012/07/01/codebender-an-online-arduino-ide/) 生成代码，毕竟[只是 C++代码](http://hackaday.com/2015/07/28/embed-with-elliot-there-is-no-arduino-language/)。

[https://www.youtube.com/embed/PcVJB9_0YnU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/PcVJB9_0YnU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)