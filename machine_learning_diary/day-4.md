# Day4：Pip这个好朋友

欢迎大家回到GirlsInAI~~

今天是machine_learning_diary的day-4，这节课我们主要讲解昨天接触过的pip安装。在之后和python打交道的过程中，这个工具会是我们的忠实伴侣。

### **初识pip**

在python的学习中，最常见的就是引入各种需要依赖的包，比如你们常常听说的numpy和pandas，还有听起来就很酷的Tensorflow等等，这就必须要和我们的好朋友pip来打声招呼了~

pip是python包管理工具，提供了对python包的查找、下载、安装、卸载的功能。

在之后的学习中，我们会依赖很多python包，比如我们常常听说的Tensorflow，matplotlib等等，这些包的安装和升级包括卸载都需要pip的帮忙来完成。

### **pip和conda的区别**

conda是另一种包管理工具。

很多同学都听说过pip和conda，但始终不明白这两个工具有什么区别，首先声明，两个工具的区别与我们之后的学习和使用关系并不大，使用哪个都可以~这节课我们只介绍pip，如果对于pip使用失败时也可以自主尝试使用conda。之后我们会具体介绍的~

了解两者区别是因为我们对知识有强烈的好奇心！对的就是这样！

主要区别有两点：

1. conda是主要针对数据领域的，而pip不是。
2. conda不仅仅包含python包，也包含非python的工具，而pip只针对python。

接下来我们看看pip的一些最基本操作吧~

### **用pip来安装包**

在讲如何用pip来安装包之前，先举个例子，我们在python中是如何使用这些包的（涉及之后课程的一点知识，主要是为了做个对比更容易理解~）

我们打开Jupyter，然后输入：import numpy，点击run。（目前你们只需要了解numpy是进行数学操作的，详细的我们会之后再讲~）

![img](http://img.xiumi.us/xmi/ua/139aW/i/ee4a6c4c92f1e36861ab608cd3fc55ce-sz_19656.png)

红色的ModuleNotFoundError的意思是这是一个找不到包的错误，这时候我们就需要pip的帮忙了~

当我们想要安装某些包时，需要知道导入包的名称，然后在pip.exe的目录下（如果你现在使用Jupyter进入终端就忽略pip.exe这个问题），在终端中输入pip install (name)，回车。

我们以numpy为例。（忽略我的蓝色背景，这是直接进入想要的文件夹终端的小tip，之后我会发到微博进行知识补充~）

输入：pip install numpy，回车。

![img](http://img.xiumi.us/xmi/ua/139aW/i/1633511695e1bc6cddea7084ac31468f-sz_19685.png)

截图中可以看到，已经成功安装上numpy啦~

是不是很简单呢~

这时候再去你的Jupyter中重复我们之前导入包的动作，看看是不是结果不一样了呢~只要没有红色的ERROR就是成功了哦~

### **查看当前pip版本**

接下来我们看看如何查看pip当前版本。

用Jupyter打开Terminal（终端）

输入：pip --version，回车。

![img](http://img.xiumi.us/xmi/ua/139aW/i/4d477b784b8282742d1472ac87e57899-sz_6961.png)

可以看到我电脑中的pip版本是18.1

作业：安装pandas包

来试着独立安装一个名字叫pandas的包吧~

终端中输入：pip install pandas，回车。

![img](http://img.xiumi.us/xmi/ua/139aW/i/6a96e687227b684676afdaa01cc291d0-sz_47009.png)

在Jupyter中输入：import pandas。点击Run看看效果吧！把你们成功导入包的截图发给我们吧~

看到这，你已经算是交下pip这个朋友了，但pip的功能远不止于此，以后我们会慢慢介绍。

也许在下载，安装的过程中会遇见各种问题，我们会慢慢总结慢慢讲解的。

关于MacOS版本后续补上，有任何疑问都可以来微博/Github找我们哦。

Coding is the new sexy.

-小鹿 @Miss_Giraffe1229, 2019/01/08