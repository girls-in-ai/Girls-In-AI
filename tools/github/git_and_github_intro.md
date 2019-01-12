
# Machine Learning Diary番外工具篇之Git&GitHub简介

欢迎大家来到GirlsInAI👏

**[machine_learning_diary](https://github.com/YZHANG1270/Girls-In-AI/tree/master/machine_learning_diary)** 是人工智障工程师养成日记系列。每次的课程以日记的形式发布。希望通过每天进步一点点，成为一个AI killer😝


**今天来带大家简单认识一下Git和GitHub。**
- 1.Git & GitHub简介
- 2.安装Git
  - 2.1 MacOS版本
  - 2.2 Windows版本
  
因为这一期和machine learning本身关系不大，不过git又是工作中必须要用的东西，所以把一些基本简单的内容放在这里，供大家参考。   
<br><br>

## 1.Git & GitHub简介
简单来说，🌟GitHub 是一个网站 🌟git是一个工具。  
它们的关系可以理解为 **GitHub是百度网盘网站，Git是百度网盘管家。**  

把我们电脑里的代码 通过git这个工具 **上传**到github这个云端网站上  
把网站上的代码 通过git这个工具 **下载**到我们电脑里。  

- git是一个version control的工具  
什么是version control呢？比如我昨天写了10行代码，版本一，把这段代码上传到github上面; 今天又写了2行，一共12行，版本二，再把版本二上传到github上面 , **github会帮助我们记录每一次的更新！** 比如过段时间，我们发现，版本二中的第二行错了，导致我们整个代码不能运行，那么我们可以随时返回到版本一.  
这就是version control (我翻译为版本控制）   

- git允许多人操作  
  比如同事A在马来西亚写了版本三，同事B在中国写了版本四。那么同事A上传之后，同事B也可以在A的基础上继续写代码，然后上传到github上的同一个工作文档。 
如果大家已经注册github账号，那么我们就开始讲git吧！  
github就是一个网页，比较容易理解  
git是工具，需要一些时间，但是并不难。跟着我们一块学起来吧。   
<br><br>

## 2.安装Git  
- 检查电脑里是否已经安装Git  
这里就需要用到一个“看起来酷酷的”小程序，就是我们经常在电脑上看到的一个黑色代码方框（也有可能是白色的）  
Windows系统里这个方框叫做Command Prompt／MacOS系统里这方框叫做Terminal（终端)。下节课里我们会有跟详细的关于终端的介绍。

### 2.1 MacOS版本  
以MacOS为例，在Finder -> Applications -> Utilities找到Terminal.app, 点击打开它。
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/IMG_0729.jpg?raw=true" width="50%" height="50%" />  

在命令行输入 `git version`  
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/2.png?raw=true" width="50%" height="50%"  align="middle"/>  
如果你的电脑里面出现了git version x.xx.xx这个东西，那就说明你的电脑里已经装好git啦。
如果没有， 点击官方安装网址： [https://git-scm.com/download](https://git-scm.com/download)，选择MacOS版本，follow instructions, 很快git就会安装好。

### 2.2 Windows

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

装好了以后，大家可以通过`git version`这个指令来查看自己当前git的版本，如果显示了一个版本，说明你已经成功安装git啦~

关于git的部分我们就讲到这里。

<br><br>
<br><br>
## 3.玩转GitHub  

这一部分是关于GitHub的使用补充。

首先直接在github.com注册sign up或者登录sign in, 登录进来之后，呈现的这一个页面是我自己的首页（这是新的账号，所以可能和你们一样没有太多东西）我们来了解一下。   
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/IMG_0734.jpg?raw=true" width="50%" height="50%" />  
左侧的repository其实就是文件夹，简称repo；**这个文件夹可以自己新建，也可以copy人家的文件夹**
<br><br>
### 3.1 新建自己的repo  
点击Start a project  
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/6.png?raw=true" width="50%" height="50%" />  
- 出现这个页面，首先为你的Repository取名字（按你们的喜好来就好了）
- description是可选项，就是用来简单描述你这个文件夹的作用性质 
- Private是收费项目，这样其他人不能看到你的文件夹内容

- 一般是Public,所以大家可以共享你的资源
- 下一个选项README, 就是一个文件，你们可以把它想做word文档，用来具体描述这个文件夹的作用性质 (read me读我嘛）可选可不选。选了之后会自动在你的文件夹里面生成这样一个空文档，自己去填写内容。 
- 下面两个我们先不选择，它就是让你为你的文件夹选择编程语言之类的。 
- 然后点击Create Repository 
然后就自动跳转到这个页面，voila, 这就是你自己在github上的文件夹啦。 
![]<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/7.png?raw=true" width="50%" height="50%" />  
<br><br>

## 写在后面：  
之前说过，我们既可以从github下载到我们电脑，也可以把电脑的东西上传到github。  
下一课我们会讲更多关于Terminal的用途喔，敬请期待~

Keep Calm and Code On!





