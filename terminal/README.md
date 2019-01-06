# 用终端来下载GirlsInAI的学习资料

简单地说，终端是一种用于执行系统命令行指令的程序。在MacOS系统里，这个终端程序被称作Terminal，在Windows系统里，常用的终端程序是Command Prompt。命令行能够帮助我们执行很多图像界面不提供的功能，是软件开发里必不可少的工具。这一课我们教大家如何使用MacOS系统自带的Terminal程序来下载GirlsInAI的学习资料。

## MacOS版本

## Step 1 -- 打开Terminal程序

在Finder -> Applications -> Utilities里面找到Terminal.app，点击打开。

或者通过右上角的搜索直接搜“Terminal", 按下回车键就能直接打开。

当Terminal程序打开后，建议大家选择把Terminal放在Dock里面，因为之后我们会经常用到它。

## Step 2 -- 打开/新建一个用来存储学习资料的文件夹

在Terminal程序里，有两个基本的指令需要大家记住：
cd   帮助我们去到想去的文件夹
mkdir  帮助我们创建新的文件夹

在这里为了个大家演示，我选择在自己的Documents文件夹里创建一个新的文件夹叫Demo
cd Documents
mkdir D

## Step 3 -- 复制一个Git Repo到自己的电脑里 （Clone a Git Repository to your local machine）

当你从git上面clone一个repo (大家可以暂时想象成从一个遥远的地方拷贝一个文件夹到你自己的电脑上）时，它会自动帮你创建一个和这个repo同名的文件夹，里面包含着这个repo下面的所有内容。

首先我们回到GitHub GirlsInAI的repo, 在下图的标注的位置有一个绿色的Clone or download按钮，按下这个键之后，会出现一个Clone with HTTPS的信息框，我们点击右边这个复制小按钮，就把GirlsInAI的repo地址存在了剪贴板。

这时我们回到Terminal, 输入git clone command+v (粘贴repo地址），按下回车键，系统就会自动复制GirlsInAI的repo内容。这时大家可以通过Finder里面的文件夹，找到GirlsInAI这个文件夹，看看是不是包含了和GitHub上面一样的内容呢^_^

如果你成功找到了这个文件夹，并且可以看到里面的文件，恭喜你呀，你已经学会如何通过Terminal来复制一个Git Repo啦！

## Step 4 -- Fetch Future Changes

通过Step 3,我们成功复制了当前时刻的repo到自己的电脑上，那么之后我们有更多的学习内容被添加进去的时候，是不是每一次都要重新复制这个repo呢？

当然不用那么麻烦！这里就是git发挥它的神奇功效的地方了。通过Terminal，大家可以看到你现在是在一条叫master的branch上面，以后每次有新的内容被添加到这条branch的时候，你都可以通过
git pull 的指令来fetch当前最新的内容呢。

在以后的课程中，我们也会不断帮大家学习新的git指令，敬请期待吧~~~

谢谢你看到这里，如果在安装过程中遇到什么样的困难，也可以在微博或者GitHub上面留言给我。







