
# Git&GitHub

欢迎大家来到GirlsInAI👏

**[machine_learning_diary](https://github.com/YZHANG1270/Girls-In-AI/tree/master/machine_learning_diary)** 是人工智障工程师养成日记系列。每次的课程以日记的形式发布。希望通过每天进步一点点，成为一个AI killer😝


**今天来带大家简单认识一下Git和GitHub。**
- 1.Git & GitHub简介
- 2.安装Git
- 3.玩转Git & GitHub
  - 3.1新建自己的repo
  - 3.2下载Girls-In-Ai repo  
    - 🚩简单的命令操作
    - 🚩更新本地文件夹
  
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
git是工具，需要一些时间，但是并不难。跟着我一块学起来吧。   
<br><br>
## 2.安装Git  
- 检查电脑里是否已经安装Git  
这里就需要用到一个“看起来酷酷的”小程序，就是我们经常在电脑上看到的一个黑色代码方框（也有可能是白色的）  
Windows系统里这个方框叫做Command Prompt／MacOS系统里这方框叫做Terminal（终端）  
以MacOS为例，在Finder -> Applications -> Utilities找到Terminal.app, 点击打开它。    
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/IMG_0729.jpg?raw=true" width="50%" height="50%" />  
  
在命令行输入 `git version`  
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/2.png?raw=true" width="50%" height="50%"  align="middle"/>  
如果你的电脑里面出现了git version x.xx.xx这个东西，那就说明你的电脑里已经有git了，可以直接跳到下一步   
（发现自己这个电脑已经很久没更新git了 lolll ) ；   
如果没有，那我们在chrome页面输入 download git, 点击这个官方网站，根据你的需求下载macos/windows的git, 安装包（30多MB) 下载好之后，就直接“下一步”，“下一步”即可  
<br><br>
<br><br>
## 3.玩转Git & GitHub  
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
### 3.2 下载Girls-In-Ai repo  
之前说了嘛，GitHub只是一个云端网站，以把网站的东西下载到电脑上。让我们来看一看，怎么把我们创建的这个文件夹放到我们的电脑上呢？   
让我们返回Terminal 直接输入git，启动git 
我们先来认识一下这一排命令行。
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/8.png?raw=true" width="50%" height="50%" />  
冒号之前是我的电脑名称，冒号之后是我们所处的的电脑文件夹位置，然后我的账户名称，最后就可以输入命令行了   
  
#### 🚩几个简单的命令操作  
- 1.～ （是我们的”电脑主页“
- 2.ls （list, 显示你现在所在的文件夹包含的内容）  
  <img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/9.png?raw=true" width="50%" height="50%" />  
  可以看到在”~”这个最外面的电脑文件夹里，还有这些子文件夹。   
- 3.cd + 文件夹名称 （change the directory 我们可以跳转到任意一个子文件夹）  
  例如我想去Documents这个文件夹 那就cd Documents  
  <img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/IMG_0741.jpg?raw=true" width="50%" height="50%" />  
  你看 “~”这里就变成了Documents,显示你现在所在的文件夹位置，同样可以ls查看里面有什么文件，🌟如果你想返回上层，返回上一个文件夹，就用 cd ..即可  
- 4.mkdir +你想要的文件夹名称 (新建文件夹)  
  如果我们想在Documents文件夹这里新建一个用来储存我们刚刚新建的repo，就可以mkdir GitTest。然后进入这个GitTest,看一下里面有什么内容吗？  
  <img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/10.png?raw=true" width="50%" height="50%" />   
  因为是个空文件夹，所以不会显示任何东西  
- 5.git clone + repo地址（从github上下载我们新建的repo）  
  首先回到我们新建的repo页面，然后点击clone or download（克隆和下载）复制我们这个repo的地址  
  <img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/IMG_0744.jpg?raw=true" width="50%" height="50%" />    
  然后在命令行里直接git clone + 粘贴  
  <img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/11.png?raw=true" width="50%" height="50%" />   
  然后我们回到finder，就可以看到我们的GitTest文件夹和里面空空的README文件啦。  
  <img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/12.png?raw=true" width="50%" height="50%" />   
<br><br>
  **同样的道理，如果你们想把Girls-In-AI的内容下载到你的电脑里**  
  先找到我们的repo，直接搜索Girls-In-AI  
  <img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/13.png?raw=true" width="50%" height="50%" />   
  然后复制我们的repo地址，选择你想要储存的文件git clone到你的电脑即可
  <img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/14.png?raw=true" width="50%" height="50%" />   
  <img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/15.png?raw=true" width="50%" height="50%" />   
  你们看现在我们的Girls-In-AI就在我们的电脑里面啦  
  <img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/16.png?raw=true" width="50%" height="50%" />   

#### 🚩更新本地文件夹  
如果后续我们的Girls-In-AI有更新，你也想把这个更新同步到你的电脑里，可以直接用git pull这个指令  
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/git_intro/17.png?raw=true" width="50%" height="50%" />   
因为我们刚刚才下载好这个文件，所以肯定是最新版本Already up-to-date  
后续我们会持续更新GIA, 大家如果想同步，记得cd Girls-In-AI, 然后git pull哦   
<br><br>
<br><br>

## 写在后面：  
我之前说过，我们既可以从github下载到我们电脑，也可以把电脑的东西上传到github。  
我们上面的内容只说了从github下载到电脑，包括下载更新内容git pull  
没有讲到如果我们想把我们电脑上的东西上传，git push,因为这个和machine learning关系没那么密切，所以这里先不讲。  
大家只要记得 git pull (pull - 拉，从云端拉下来） 和git push (push - 推，把东西从本地推到云端上去）就可以啦。 





