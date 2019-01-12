# Day4：魔法口令 - “pip install xxx”

欢迎大家回到GirlsInAI~~👏

今天是machine_learning_diary的day-4，这节课主要介绍如何把别人的代码拿来自己用嘿嘿😜Python是一门伟大的语言，每天有数以万记的工程师在使用python，自然会有聪明又勤奋的工程师写出优雅又有用的代码块供大家使用，对，免费分享，这就是开源的力量！接下来的课程我也会不断带大家一步步感受开源的世界到底有！多！美！好！😍

“偷”别人写好的代码块，只需要一句魔法口令“**pip install xxx**”，这个“xxx”就是别人写好的包package的名字。



## **初识pip**

pip是python 著名的包管理工具，在python开发过程必不可少。本节带大家了解用pip实现的python包的下载、卸载、查看等详细操作。

打开你的Terminal（终端）：

- MacOS 在spotlight搜索“终端”，点击打开

- Windows 找到左下角菜单旁边的搜索圆圈输入“cmd”，回车

  ![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day4/001.jpg?raw=true)



就出现了电脑黑客必备工具，黑框框界面，也可以是白的~

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day4/002.png?raw=true)

别慌，一打开只是没有这些红框框，接下来跟着做：

1. 按照红框1号输入 ```pip```或者```pip --help```，就会出现这样的界面
2. 红框2号是 pip可以搭配的命令，比如第一个就是pip install 的“install”
3. 红框3号是每个命令相关的介绍说明
4. 下面这个红框是其他可以搭配的命令



## 查看当前pip版本 - Windows版本

好了，咱们来查看当前pip 版本，输入 ```pip --version```

然后可以看到跳出的最开始几个字母```pip 9.0.3```就是版本号，但是我们的重点是看这个pip对应的python是什么版本，在这行的最后有```python 3.5```字样，就说明对应的是python35。

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day4/003.png?raw=true)



## 查看当前pip版本 - MacOS版本

输入pip后双击Tab键，应该会出现pip3。继续输入完整命令```pip3 --version```，就能看见这个pip对应的python版本，如果是python35是正确的，如果不是，请找到你的python3.5对应的pip口令。这里假设“pip3”就是对应python3.5的pip口令。

**注意！！下面这个是重点：**

**因此，以下所有的pip相关命令，MacOS的同学都用“pip3”替换“pip”，比如**

- **Windows的同学输入命令```pip install pandas```**
- **MacOS同学对应的命令是```pip3 install pandas```**



## pip install xxx

进入正题，咱们先拿国宝级的包来试一下手，这个包就叫“pandas”，名字就说明了这个包在python届的地位，以后你会经常看见它嘿嘿~

1. 输入命令```pip install pandas```

   我是早就下载过的，你们就等待它下载完就可以了，最后会有successful字样。

2. 双重检查是否下载成功，输入命令```python```就打开python编辑器了

3. 在python里输入命令```import pandas```,尝试把这个包import进来，如果直接跳到```>>>```三个箭头让你输下一行命令，就说明你已经把pandas国宝装进你的python啦！

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day4/004.png?raw=true)

4. 继续输入```exit()```	 将退出python，重新进入到terminal的环境，可以继续下载另一个包。每个包下载完成的最后都会有“Successfully installed”字样，表示下载成功。

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day4/005.png?raw=true)



## pip uninstall xxx

很简单，uninstall的命令就是卸载一个包。大家可以自己尝试做一下。



## 作业

以后咱们会常见的包有：

- pandas
- numpy
- matplotlib

今天教了大家怎么下载国宝pandas，剩下两个自己安装，并且进入python 使用 import xxx命令检查一下。

👩好啦，今天的课程就到这里啦！咱们下次见！~