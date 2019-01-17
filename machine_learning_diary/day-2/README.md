# Day2：Python这一大家子

欢迎大家回到GirlsInAI👏

今天是 [**machine_learning_diary**](https://github.com/YZHANG1270/Girls-In-AI/tree/master/machine_learning_diary) 的day-2, 来带大家稍微认识一下Python这一大家子。python作为一门流行语言在不断迭代更新中，会有很多语言版本。今天学习如何下载一个新的编程环境以及环境配置。

注：建议大家把Chrome设为默认浏览器。



## 查看当前 Jupyter 的Python版本

用Anaconda Navigator打开python35的 Jupyter Notebook。如果你的默认浏览器是Chrome，会自动弹出：

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day1/006.png?raw=true)

点击“New”，点击“Terminal”，中文是“终端”的意思：

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day2/004.jpg?raw=true)

在新弹出来的窗口中输入“python”，就可以看到我这里当前python版本是3.6的。因为我是之前就下载了的。如果是day-1下载的：

- MacOS的同学应该是2.7的，因为MacOS自带2.7版本的python
- Windows的同学应该是3.7的，这个3.7是Anaconda自带的python版本

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day2/007.png?raw=true)





## Py2、Py3

科普时刻：

1. python作为一种编程语言有很多版本。还在不断进化中。
2. Py（或py）是python的通用缩写。“.py”是python文件的后缀。就像“.xlsx”是excel文件后缀。
3. **Py2** 和 **Py3** 是python语言的两大主流。就像繁体字与简体字的关系。
4. 目前最新的版本是Py3.7。（2019-01-07）

**接下来的课程我们推荐用py3.5，建议用py3以上，py3.6或者py3.7都可以**。所以今天我们要尝试做两件事：

- 下载python3.5的环境+配置这个环境
- 下载对应的 Jupyter Notebook



## Anaconda下载Python 3.5

Windows点击左下角菜单，点击Anaconda文件夹下的Anaconda Navigator：

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day2/001.jpg?raw=true)

MacOS点击绿色图标Anaconda Navigator点开之后你将看见：

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day2/001.png?raw=true)

1. 点击左侧菜单栏的“Environment”
2. 点击下方的“Create”
3. 在弹出的对话框选择“Python 3.5”
4. 给这个新环境命名，例如我的就很直接叫“python35”。你可以取你喜欢的代号，毕竟以后天天见。
5. 点击对话框的“Create”，完成Python3.5的下载



**注意！！接下来是Windows版本的方法介绍，MacOS的同学们请点击这个链接进行尝试：[点我！快点我！](https://github.com/YZHANG1270/Girls-In-AI/blob/master/machine_learning_diary/day-2/Python_for_MAC.md)**



## Windows 环境变量配置

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day2/002.png?raw=true)

找到你的python3.5下载到的文件夹，下图为我py35的地址：

- C:\Users\Yi\Anaconda3\envs\python35
- C:\Users\Yi\Anaconda3\envs\python35\Scripts

上面这两个地址都需要复制然后粘贴，然后看下图：



![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day2/003.png?raw=true)

1. 在“此电脑”右击选择“属性”，弹出控制面板对话框
2. 点击“高级系统设置”
3. 点击“环境变量”
4. 找到下方的系统变量方框
5. 找到“Path”，双击打开
6. 点击右侧“编辑”
7. 在第一个添加刚刚复制的python35的地址：C:\Users\Yi\Anaconda3\envs\python35
8. 点击“确定”
9. 点击“确定”
10. 点击“确定”
11. Ok，完成！



## 下载python3.5版本的 Jupyter Notebook

把新的语言下载好了，当然书写的笔记本也要更新。

点击左下角菜单，点击Anaconda文件夹下的Anaconda Prompt：

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day2/002.jpg?raw=true)

弹出一个黑框：

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day2/006.png?raw=true)

1. 输入“activate python35”，启动新环境。这里的“python35”是我取的新环境名字，你填入你取的名字。
2. 输入“pip install jupyter notebook”，进行“丘比特💘”笔记本下载。
3. 漫长的等待，直至下载完成，大功告成。





## 作业：检查 Jupyter 的 新环境

### Windows

当新的py3.5版本的Jupyter下载完之后，继续输入命令“jupyter notebook”，就能启动你的新笔记本了：

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day2/008.png?raw=true)

此时，仍然会弹出一个页面：

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day1/006.png?raw=true)

这时候你再点击“New”下面的“Terminal”，输入“python”，看看到底变成了什么版本~~🙌



### MacOS

根据Anaconda Navigator打开python35的 Jupyter Notebook

![](https://github.com/YZHANG1270/Girls-In-AI/raw/master/others/pics/ml_day1/010.jpg?raw=true)

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day1/006.png?raw=true)

打开后进入终端，键入命令```python3```查看版本。

大家有什么不懂的可以第一时间Google一下或者提issue，也欢迎来跟@Girls-In-AI分享讨论今天的内容。

👩好啦，今天的课程就到这里，咱们下期见~！