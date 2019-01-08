# Day4：Pip这个好朋友

欢迎大家回到GirlsInAI~~

今天是machine_learning_diary的day-4，这节课我们主要讲解昨天接触过的pip安装。在之后和python打交道的过程中，这个工具会是我们的忠实伴侣。

### **初识pip**

pip是python包管理工具，提供了对python包的查找、下载、安装、卸载的功能。

在之后的学习中，我们会依赖很多python包，比如我们常常听说的Tensorflow，matplotlib等等，这些包的安装和升级包括卸载都需要pip的帮忙来完成。

### **pip和conda的区别**

conda是另一种包管理工具。

很多同学都听说过pip和conda，但始终不明白这两个工具有什么区别，首先声明，两个工具的区别与我们之后的学习和使用关系并不大，使用哪个都可以。这节课我们只介绍pip，如果对于pip使用失败时也可以自主尝试使用conda。之后我们会具体介绍的~

了解两者区别是因为我们对知识有强烈的好奇心！对的就是这样！

主要区别有两点：

1. conda是主要针对数据领域的，而pip不是。
2. conda不仅仅包含python包，也包含非python的工具，而pip只针对python。

接下来我们看看pip的一些最基本操作吧~

### **查看当前pip版本**

用昨天教程中的方法打开Terminal（终端）

输入pip --version，回车。

![img](http://img.xiumi.us/xmi/ua/139aW/i/4d477b784b8282742d1472ac87e57899-sz_6961.png)

可以看到我电脑中的pip版本是18.1

### **用pip下载包**

当我们想要下载某些包时，需要知道导入包的名称，然后再pip.exe的目录下（如果你现在使用Jupyter进入终端就忽略pip.exe这个问题），在终端中输入pip download (name)，回车。

我们以tensorflow为例。（忽略我的蓝色背景，这是直接进入想要的文件夹终端的小tip，之后我会发到微博进行知识补充~）

输入：pip download tensorflow，回车。

![img](http://img.xiumi.us/xmi/ua/139aW/i/e5a1665f2640663be1adfe32d97b0084-sz_176989.png)

![img](http://img.xiumi.us/xmi/ua/139aW/i/f296f4cb96b62fefdb75cc2c76e90972-sz_107524.png)

由截图我们可以看到，当我们想让pip安装tensorflow包时，它自主的去网络上收集需要的文件并下载。第二张截图中能看到最后一行的successfully证明下载成功。

### **用pip来安装包**

我们已经下载了需要的安装包，现在可以使用pip来安装啦~

依然是在pip.exe的目录下（或者通过Jupyter），在终端输入pip install (name)，回车。

继续以tensorflow为例。

输入：pip install tensorflow，回车。

大家可以看到截图中，pip列出了tensorflow需要的安装环境，并一一准备好，最后的提示是说明我的电脑中已经存在tensorflow了。

![img](http://img.xiumi.us/xmi/ua/139aW/i/3fa5af0da2a3b6cd2fc9a290c8ad5ce3-sz_108196.png)

看到这，你已经算是交下pip这个朋友了，但pip的功能远不止于此，以后我们会慢慢介绍。

也许在下载，安装的过程中会遇见各种问题，我们会慢慢总结慢慢讲解的。

关于MacOS版本后续补上，有任何疑问都可以来微博/Github找我们哦。

Coding is the new sexy.

-小鹿 @Miss_Giraffe1229, 2019/01/08
