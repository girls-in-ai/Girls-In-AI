###  machine_learning_diary/day-3
今天也是学习的一天， 之前学的python知识， 由于不常运用， 渐渐就会遗忘， 结合工程是最好掌握一门语言的方法（奈何现在只做了java的工程）

这次课程带我回顾了变量的知识

**conception**
- 变量：
*variables are reserved memory locations to store values*
变量是预留的内存地址，用来存储值
（可以看成是个杯子， 可以放许多不同数据类型的东西  比如：Numbers数字（1）、String字符串 （"girls in AI"）

**Python Numbers**

Number data types store numeric values. **Number objects are created when you assign a value to them.**

Number类型用来存数字值。 *Number对象在你赋给它们值时被创建*

For example −
```
var1 = 1
var2 = 10 #var1是一个Number类型的对象
```
You can also delete the reference to a number object by using the del statement. The syntax of the del statement is −

你也可以通过用**del**来删除指向number 对象的引用
```
del var1[,var2[,var3[....,varN]]]]
```
You can delete a single object or multiple objects by using the del statement.

你可以通过用**del**删除一个或多个对象

For example −
```
del var
del var_a, var_b
```
### 参考链接
[Variable Types](https://www.tutorialspoint.com/python3/python_variable_types.htm)

[数据模型](https://docspy3zh.readthedocs.io/en/latest/reference/datamodel.html)

一贯的遇到了很多问题（就是不断会遇到问题的， 大家放宽心）

**issues:**
由于我之前下载了python2.7、3.7、3.6，现在又下了3.5 。。。。 所以环境变量一大堆， 很容易出现版本冲突， 在这里告诉大家一个可以切换python版本的方法。

1. 首先大家可以找到自己下载python的文件所在地（路径），以我的为例：

![](https://img-blog.csdnimg.cn/20190115180152701.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)

大家注意到， 这里python的exe文件名字被我改成了python3, 所以 如果我想用3.6版本的python， 我就会在命令行中输入python3, 这时它的版本就是3.6的， 可以使用python --version来查看。![](https://img-blog.csdnimg.cn/20190115180434327.png)

我这里还有一个2.7版本的python, 大家可以猜到， 如果我输入python2的话， 版本会是？

![](https://img-blog.csdnimg.cn/20190115180500703.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)

![](https://img-blog.csdnimg.cn/20190115180633866.png)

2. 但是如果你要使用pip命令下载其他人的模块， 就要注意环境变量的配置了。
**设置环境变量**（Windows10）
右键我的电脑->属性->高级系统设置->环境变量
在下方的**系统变量**中，找到Path, 双击

![](https://img-blog.csdnimg.cn/20190115181332588.png)

这里我想要用python3.5版本的pip， 所以要把它的路径上移到最上面
![](https://img-blog.csdnimg.cn/20190115181428658.png)

![](https://img-blog.csdnimg.cn/20190115181515974.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)

其实我们要做的就是， 让计算机能够找到你的pip所在的地方， 也就是设置环境变量。

推荐一个代码可视化的网站， 可以将你建立变量、赋值通过图像描绘。 [点击这个链接](http://pythontutor.com/)
