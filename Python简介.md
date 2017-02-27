# Python 简介
Python是一门面向对象的编程语言。具有比较广泛的用途。
* 解释性：速度偏慢；开发周期短，调试容易。
* 面向对象：类，函数，模块等都是对象。
* 可扩展：Python使用C语言写的。
* 可嵌入：Python的解释器引擎很容易的嵌入到自己的C/C++语言的项目中。
* 动态类型：不需要事先声明变量的类型。
* 强类型：一旦变量有了值，那么这个变量是有一个类型的。不能将string类型的变量直接赋值给一个integer类型的变量，而是需要类型转换。

# 语言解释器
* CPython

当我们从Python官方网站下载并安装好Python 2.7后，我们就直接获得了一个官方版本的解释器：CPython。这个解释器是用C语言开发的，所以叫CPython。在命令行下运行python就是启动CPython解释器。

CPython是使用最广的Python解释器。教程的所有代码也都在CPython下执行。
* IPython

IPython是基于CPython之上的一个交互式解释器，也就是说，IPython只是在交互方式上有所增强，但是执行Python代码的功能和CPython是完全一样的。好比很多国产浏览器虽然外观不同，但内核其实都是调用了IE。

CPython用>>>作为提示符，而IPython用In [序号]:作为提示符。
* PyPy

PyPy是另一个Python解释器，它的目标是执行速度。PyPy采用JIT技术，对Python代码进行动态编译（注意不是解释），所以可以显著提高Python代码的执行速度。

绝大部分Python代码都可以在PyPy下运行，但是PyPy和CPython有一些是不同的，这就导致相同的Python代码在两种解释器下执行可能会有不同的结果。如果你的代码要放到PyPy下执行，就需要了解PyPy和CPython的不同点。
* Jython

Jython是运行在Java平台上的Python解释器，可以直接把Python代码编译成Java字节码执行。
* IronPython

IronPython和Jython类似，只不过IronPython是运行在微软.Net平台上的Python解释器，可以直接把Python代码编译成.Net的字节码。
* 小结

Python的解释器很多，但使用最广泛的还是CPython。如果要和Java或.Net平台交互，最好的办法不是用Jython或IronPython，而是通过网络调用来交互，确保各程序之间的独立性。