欢迎各位来到GirlsInAI~

本文是对之前的关于mac系统下git的介绍和git终端的使用进行基于windows系统下的补充。



Step 1. 下载

安装环境：win10，64bit

下载地址：https://git-scm.com/download

![img](http://img.xiumi.us/xmi/ua/139aW/i/f225b8288d096329b25a60f7e930df1b-sz_146323.png)



Step 2. 安装

开始安装的界面：

![img](http://img.xiumi.us/xmi/ua/139aW/i/826f005671bf8f0d45cbdaf8885616ea-sz_32280.png)



安装路径：

![img](http://img.xiumi.us/xmi/ua/139aW/i/87475b7cf6d399f7b5b074de91355e41-sz_20897.png)



由于已安装了git的电脑重新安装时候不再显示安装路径，所以搬运了张图片~

（此图片来自于https://www.jianshu.com/p/414ccd423efc）

路径可以自由决定安装在C盘还是D盘。



安装组件：

![img](http://img.xiumi.us/xmi/ua/139aW/i/e2faf35e66f1c8158c0ba41f0c312731-sz_30074.png)



Additional icons--On the Desktop是选择是否在桌面上创建git的图标方便使用。

Use a TrueType font in all console windows是在windows控制台使用TrueType字体。

Check daily for Git for Windows updates是日常检查版本更新。

除了默认选择的几项以外，其余的可以根据自己的需要来选择。

我自己的选择是只选了默认几项，完全可以进行正常操作。



默认编辑器：

![img](http://img.xiumi.us/xmi/ua/139aW/i/078ebd0d4265bd63b59080f319a7399d-sz_31988.png)



默认的是Vim编辑器，我个人选择了这一项。



修改系统环境变量：

![img](http://img.xiumi.us/xmi/ua/139aW/i/5c35c875c0f49c74a69332e615fba277-sz_36098.png)



第一项：只使用Git Bash，是最安全的。

第二项：使用Git Bash和命令行都可以控制Git。（我默认选择了这一项，因为需要用终端来控制git）

第三项：要修改windows控制台指令，不安全不建议选择。



SSL的证书选择：（选择默认项）

![img](http://img.xiumi.us/xmi/ua/139aW/i/b5a45c1caa3a6b651b281099a98ed535-sz_26219.png)



配置行尾结束符：（选择默认项）

![img](http://img.xiumi.us/xmi/ua/139aW/i/e808739f1fc9b75526733850f0355d6b-sz_36794.png)



配置终端仿真：（选择默认项）

![img](http://img.xiumi.us/xmi/ua/139aW/i/3aa4d2a9e47359ef2a0e8d930d591bb7-sz_36745.png)



一些其他配置：（选择默认项）

![img](http://img.xiumi.us/xmi/ua/139aW/i/9e0652cfb056f7ea11a75cd94d713937-sz_35557.png)



终于开始安装啦~~：

![img](http://img.xiumi.us/xmi/ua/139aW/i/dfc8e1a420b0330904a3c30840bc5fda-sz_15506.png)



是不是还是很简单的，接下来我们尝试用终端和git对一下话~

首先我们先来看一下如何在windows系统下打开终端。



Step 3.初识终端

windows的左下角有一个开始菜单，一个放大镜图标，不要犹豫，点击它~

![img](http://img.xiumi.us/xmi/ua/139aW/i/55de463242617687f900299fd1820cbd-sz_6642.png)



在搜索的界面上输入cmd，回车，windows就get到了你要找终端的命令了。

![img](http://img.xiumi.us/xmi/ua/139aW/i/848d4724a0945456b068f92ff6a31305-sz_30979.png)



终端的样子：

![img](http://img.xiumi.us/xmi/ua/139aW/i/cf799b96c4c603c6651d312efe142542-sz_21844.png)



Step 4. 对话git

接下来我们尝试和git打个招呼，在终端中输入git，回车：

![img](http://img.xiumi.us/xmi/ua/139aW/i/3564d2e43b80b4bf42ac7e279b7833cd-sz_90386.png)



看到这要恭喜你已经成功安装了git，并且和它say了hello~ 它给了你一个菜单，类似一个使用说明，介绍了它有什么功能，可以怎样使用，我们今天只讲几个最简单的介绍，以后都会详细讲解。

我们可以问一下git现在是什么版本，输入git --version，回车：

![img](http://img.xiumi.us/xmi/ua/139aW/i/99124139b97c4526d8c91862a7529f19-sz_4854.png)



Step 5. 新建/打开文件夹

在终端中有两个最基本的指令：

![img](http://img.xiumi.us/xmi/ua/139aW/i/3ef7ad1bb611fac7241ab3cd741ae9c0-sz_4296.png)

mkdir是新建文件夹。

cd是进入到某个路径。

图中例子是在D盘里新建了一个叫GirlsInAI的文件夹，并进入其中。



Step 6. 获取一个repo到文件夹中

当你想从感兴趣的git界面中获取需要的文件时，会发现github界面上clone功能，它会自动帮你创建一个和文件同名的文件夹，里面包含着文件里的所有内容。

具体操作步骤如下：

1. 打开github，找到GirlsInAI页面。
2. 点击图中Clone or download

![img](http://img.xiumi.us/xmi/ua/139aW/i/277fd66a2126707db6238ebab8f85f57-sz_9187.png)

​     \3. 复制地址。

​     \4. 在终端输入git clone+复制的地址回车（此处不要写“+”哦，只用空格就好）。

![img](http://img.xiumi.us/xmi/ua/139aW/i/0a467caba8a981d0e30c0f0734504e38-sz_24861.png)

现在查看一下刚刚新建的文件夹，是不是里面有了github上看到的所有内容。如果你能找到，说明你的第一个用终端操作git的例子已经完成的很好啦~撒花~~

是不是还挺简单的，那我们讲今天的最后一个操作啦~



Step 7. 获取更新内容



我们已经成功复制了想要的文件，一般在github上的项目都会持续更新，我猜你会问是不是每一次获取文件都要这么麻烦。

答案是当然不用了！git上的pull功能可以获取你想要的文件的所有更新。

在终端里，进入到你获取的文件夹中，有.git文件的目录下，输入git pull指令，回车。

![img](http://img.xiumi.us/xmi/ua/139aW/i/1c565c636c66e515c6c41e7b9c7c3686-sz_3430.png)

图中的例子是git告诉你，你已经下载了最新版的内容~

看过了今天的讲解是不是觉得终端和git也没有那么神秘，之后的课程中，我们会学习更多的git指令，一起加油吧~~

如果你在看这篇教程时有任何疑问都可以来微博/Github上提问。

Coding is the new sexy.

-小鹿 @Miss_Giraffe1229, 2019/01/07
