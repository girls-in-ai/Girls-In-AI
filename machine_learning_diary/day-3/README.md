# Day3：Python入门之变量/Variable

欢迎大家回到GirlsInAI👏

今天是 **[machine_learning_diary](https://github.com/YZHANG1270/Girls-In-AI/tree/master/machine_learning_diary)** 的day-3, 来带大家学习变量和如何在Python中创建新变量。

变量是计算机编程中一个很基础的概念，在计算机程序中，variables are reserved memory locations to store values. 当你新建一个variable的时候，你就在存储空间里预留了一部分位置。在计算机程序中，变量不仅可以是数字，也可以是任意的数据类型。具体的关于数据类型的部分，我们今天会接触到一点点，以后还会有深入展开的教程。

话不多说，我们先来通过几个小例子来理解变量这个概念吧！

### Example 1
请大家按照Day-2教的方法，打开Anaconda Prompt黑框，输入：

- activate python35(用你自己的环境名替换) 
- jupyter notebook

打开Jupyter Notebook，输入下面这行代码，我们就创建了一个叫做message的变量。

```sh
message = 'I am learning Python'
```
之后我们再输入
```sh
print (message)
```
就会看到一行内容被print出来啦！


下面是我的代码和运行结果：

![](https://github.com/qingdoua/Girls-In-AI/blob/master/others/pics/ml_day2/message.png?raw=true)

记得代码`从上往下一行一行`运行喔！

在Python中， `=`用来给变量`赋值`。在这个例子中，我们给message这个变量赋予了‘I am learning Python'这个值。在我们执行
```sh
message = 'I am learning Python'
```
这行代码的时候，Python做了两件事情：1是在内存中创建了一个叫做message的变量和一个‘I am learning Python’的字符串；2是把message这个变量指向‘I am learning Python'这个字符串。

### Example 2
我们再来创建另外一个变量
```sh
num = 2019
```
同样我们可以print出这个变量的值来
```sh
print(num)
```

![](https://github.com/qingdoua/Girls-In-AI/blob/master/others/pics/ml_day2/num.png?raw=true)

看到这一步，你是不是觉得有点太简单了呢？我们创建了一个叫做num的变量，然后呢？
别着急，下面我们用num来print出一个新的数值吧
```sh
newNum = num + 100
print(newNum)
```
再看看这次print出来的结果，有什么不一样呢？

![](https://github.com/qingdoua/Girls-In-AI/blob/master/others/pics/ml_day2/newNum.png?raw=true)

在上面这一段代码里，我们在num这个变量的基础上，同个`+`这个操作，创建了一个新的变量，在这里这个`+`被称作`operator`, 今天只是简单的介绍，在以后的课程中我们会学到更多的operators.

通过上面的两个例子，大家学会如何创建变量了吗？你也可以试着自己创建一些有趣的变量，来熟悉今天学到的知识喔。

Python一门很特殊的语言，它使用`object(对象)`这个概念来实现对数据的抽象。上面我们创建出的几个变量，`message`, `num`, 以及`newNum`，在Python中都被称作对象。至于对象的类型和其他特性，我们会在以后的课程中慢慢展开。

### Future Reading
如果你想学习了解更多关于Python变量的知识，可以通过下面几个网站：
https://www.tutorialspoint.com/python3/python_variable_types.htm
https://docspy3zh.readthedocs.io/en/latest/reference/datamodel.html

好啦今天的课程就到这里了，希望大家学得愉快，也欢迎大家在微博上面和我们互动，下期见~

`It's a beautiful day to write some code!`

-青豆 @ Seattle, 2019/01/06




