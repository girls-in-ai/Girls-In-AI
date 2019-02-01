[Git帮助手册](https://git-scm.com/book/en/v2)

git命令全面介绍， 可以选择中文版阅读(不过有些内容有丢失， 如果能看懂原版， 建议看原版)

创建一个版本控制的文件, 用到的这些git指令， 可以对照着手册进行阅读
- git init
- git add
- git commit
- git push

今天尝试git commit, 提示我有untracked file

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190130211555101.png)

有些疑惑， 于是去查看了git帮助手册
在第一章<a href="https://git-scm.com/book/en/v2/Getting-Started-Git-Basics">1.3 git basics</a> 中， 了解到了git的三种状态
- committed(已提交)
- modified(已修改)
- staged(已暂存)

下面看看手册中如何解释这三个状态

- Committed means that the data is safely stored in your local database.
committed意味着数据被安全的存储在你的本地数据库中

- Modified means that you have changed the file but have not committed it to your database yet.
modified意味着你已经改变了你的文件但是还没有把改变提交到你的数据库中

- Staged means that you have marked a modified file in its current version to go into your next commit snapshot.
staged意味着对一个已修改文件的当前版本做了标记，使之包含在下次提交的快照中。（个人理解， 就是修改的文件准备好要被提交（commit）了）

由此引入 Git 项目的<a id="concept">三个工作区域的概念</a>：Git 仓库（the Git directory,） 工作目录（ the working tree）以及暂存区域（the staging area.）.

![](https://img-blog.csdnimg.cn/2019013021332733.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)

- The Git directory is where Git stores the metadata and object database for your project. This is the most important part of Git, and it is what is copied when you clone a repository from another computer.                                                                  
**(Git directory)** 是 Git 用来保存项目的元数据和对象数据库的地方。 这是 Git 中最重要的部分，从其它计算机克隆仓库时，拷贝的就是这里的数据。

- The working tree is a single checkout of one version of the project. These files are pulled out of the compressed database in the Git directory and placed on disk for you to use or modify.                                                                                    
**Working directory**（工作目录）是对项目的某个版本独立提取出来的内容。 这些从 Git 仓库的压缩数据库中提取出来的文件，放在磁盘上供你使用或修改。（我理解为自己电脑上本地磁盘上的文件）

- The staging area is a file, generally contained in your Git directory, that stores information about what will go into your next commit. Its technical name in Git parlance is the “index”, but the phrase “staging area” works just as well.                              
**staging area**(暂存区域)是一个文件，它保存了下次将提交（commit）的文件列表信息，一般在 git directory中。 有时候也被称作索引‘(index)’，不过一般说法还是叫暂存区域(staging area)。

The basic Git workflow goes something like this:
基本的 Git 工作流程如下：

You modify files in your working tree.                                                                                                    
你修改的文件在 **working tree(工作目录)**中  (也就是你在本地磁盘上想要版本控制的那个文件）

You selectively stage just those changes you want to be part of your next commit, which adds only those changes to the staging area.      
选择暂存那些你*想放到下一次提交（commit）的改变*，将文件快照（也就是改变后的文件）

You do a commit, which takes the files as they are in the staging area and stores that snapshot permanently to your Git directory.        
**提交更新**，找到*暂存区域（staging area）*的文件，将快照永久性存储到**Git 仓库目录。**(git directory)

If a particular version of a file is in the Git directory, it’s considered committed.                                                      
如果 Git 目录中保存着的特定版本文件，就属于**已提交状态(committed)。**

If it has been modified and was added to the staging area, it is staged.                                                                            
如果作了修改并已放入暂存区域，就属于**已暂存状态(staged)**。

And if it was changed since it was checked out but has not been staged, it is modified.                                                            
如果自上次取出后，作了修改但还没有放到暂存区域，就是**已修改状态。(modified)**


回到刚刚我遇到的问题，提示我nothing added to commit but untracked files present
没有被加到提交(commit)中的文件， 但是有untraked(未跟踪)的文件
为了知道这个未跟踪是什么意思， 我又找到了另一节内容。

第二节内容大致概括了Git的大部分操作， 推荐初学者看。

**2.1 Git Basics - Getting a Git Repository**
**2.2 Git Basics - Recording Changes to the Repository**

![](https://img-blog.csdnimg.cn/20190131171401847.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)

### 1. Getting a Git Repository

有两种取得 Git 项目仓库的方法。 
- 第一种是在现有项目或目录下导入所有文件到 Git 中；                                                                                                     
 You can take a local directory that is currently not under version control, and turn it into a Git repository, or

- 第二种是从一个服务器克隆一个现有的 Git 仓库。                                                                                                         
You can clone an existing Git repository from elsewhere.

#### Initializing a Repository in an Existing Directory                                                            
如果你打算使用 Git 来对现有的项目进行管理，你只需要进入该项目目录并输入：

```
$ git init
```

> 注意现在是在GitTest这个上级目录中做版本控制， 所以要在GitTest上右键，点击 git bush.

![.git目录](https://img-blog.csdnimg.cn/20190131172944896.png)

该命令将创建一个名为 .git 的子目录，这个子目录含有你初始化的 Git 仓库中所有的必须文件，这些文件是 Git 仓库的骨干。 但是，在这个时候，我们仅仅是做了一个**初始化**的操作，你的**项目里的文件还没有被跟踪**。                                                                                                
This creates a new subdirectory named .git that contains all of your necessary repository files — a Git repository skeleton. At this point, **nothing in your project is tracked yet**. 

*所以这里推断出， nothing added to commit but untracked files present 是因为我做了修改的东西没有添加到暂存区域（staging area）*
【之后会说到这个暂存区域， 大家多看上面两张图， 就可以理解清楚Git的基本操作原理】

如果你是在一个*已经存在文件的文件夹*（而不是空文件夹）中初始化 Git 仓库来进行版本控制的话，你应该开始跟踪这些文件并提交。 你可通过 **git add** 命令来实现对指定文件的跟踪，然后执行 git commit 提交：                                                                                               
If you want to start version-controlling existing files (as opposed to an empty directory), you should probably begin tracking those files and do an initial commit. You can accomplish that with a few git add commands that specify the files you want to track, followed by a git commit:

```
$ git add gittest
$ git commit -m 'initial project version'
```

如下图， 执行**git add**后， 我的名为gittest的文件就会被跟踪(track), 也就是把它状态变为staged, 也就把它放入了staging area(暂存区域).

![track gittest dir](https://img-blog.csdnimg.cn/20190131173712856.png)

<a id="pic">三种工作目录与四种文件状态</a>

![在这里插入图片描述](https://img-blog.csdnimg.cn/2019013117383984.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)

![进入staging 工作区](https://img-blog.csdnimg.cn/20190131173927498.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)                                                                                                                                          
稍后我们再逐一解释每一条指令的意思。现在，你已经得到了一个实际维护（或者说是跟踪）着若干个文件的 Git 仓库。                                                  
We’ll go over what these commands do in just a minute. At this point, you have a Git repository with tracked files and an initial commit.


**Git 建立 Local Repository**
```
$ mkdir project; cd project #或者手动创建一个本地文件夹， 用右键git bush
$ git init
$ echo "hello" > hello.txt
$ git add .             #将修改（modified）过的文件添加到暂存区(staging area)
$ git commit -m 'initial' #提交commit, 初始化提交信息。
```

发现一个比较详细的git命令举例：[link](https://blog.longwin.com.tw/2009/05/git-learn-test-command-2009/)

\> 和 >> 的 区别: [What is difference between > and >>](https://stackoverflow.com/questions/39024073/using-echo-what-is-difference-between-and)

#### Cloning an Existing Repository

如果你想获得一份**已经存在了的 Git 仓库的拷贝**，比如说，你想为某个开源项目贡献自己的一份力，这时就要用到 git clone 命令。 如果你对其它的 VCS 系统（比如说Subversion）很熟悉，请留心一下你所使用的命令是"clone"而不是"checkout"。 这是 Git 区别于其它版本控制系统的一个重要特性，Git 克隆的是该 Git 仓库服务器上的几乎所有数据，而不是仅仅复制完成你的工作所需要文件。 当你执行 git clone 命令的时候，默认配置下远程 Git 仓库中的每一个文件的每一个版本都将被拉取下来。 事实上，如果你的服务器的磁盘坏掉了，你通常可以使用任何一个克隆下来的用户端来重建服务器上的仓库（虽然可能会丢失某些服务器端的挂钩设置，但是所有版本的数据仍在。

克隆仓库的命令格式是

```
git clone [url] 。
```

以Girls In AI 项目为例：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190131175102655.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190131175200546.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)

之后在命令行输入

```
git clone https://github.com/Jane-QinJ/Girls-In-AI.git
```

Git 支持多种数据传输协议。 上面的例子使用的是 https:// 协议，不过你也可以使用 git:// 协议或者使用 SSH 传输协议，比如 user@server:path/to/repo.git 。

### Recording Changes to the Repository
记录每次更新到仓库

这个算是版本控制最常用的功能了， 就是记录你的每一次修改。 你还可以为每一次修改添加必要的批注， 每一次的修改都会以快照的形式记录， 所以随时可以恢复成上一状态。

再回顾上面的图，使用 Git 时文件的生命周期如下：

![The life cycle of Git's file](https://img-blog.csdnimg.cn/20190131180007227.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)

下面详细介绍一下这几个Git中的文件状态：

Remember that each file in your **working directory** can be in one of two states:  **tracked or untracked.**                                     
请记住，你工作目录下的每一个文件都不外乎这两种状态：**已跟踪或未跟踪。**                                                                        
- Tracked files are files that were in the last snapshot; they can be unmodified, modified, or staged. In short, tracked files are files that Git knows about.                                                                                                                     
**已跟踪（Tracked ）**的文件是指那些*被纳入了版本控制的文件，在上一次快照中有它们的记录*，在工作一段时间后，它们的状态可能处于未修改（unmodified），已修改（modified）或已放入暂存区（staged）。                                                                                          
- Untracked files are everything else — any files in your working directory that were not in your last snapshot and are not in your staging area. When you first clone a repository, all of your files will be tracked and unmodified because Git just checked them out and you haven’t edited anything.                                                                                                                 
工作目录中*除已跟踪文件以外的所有其它文件*都属于**未跟踪文件（untracked）**，它们既不存在于上次快照的记录中，也没有放入暂存区。 初次克隆某个仓库的时候，工作目录中的所有文件都属于已跟踪文件，并处于未修改状态。                                                                                                        

As you edit files, Git sees them as modified, because you’ve changed them since your last commit. As you work, you selectively stage these modified files and then commit all those staged changes, and the cycle repeats.                                                               
编辑（edit）过某些文件之后，由于自上次提交后你对它们做了修改，Git 将它们标记为已修改文件（modified）。 我们逐步将这些修改过的文件放入暂存区(staging area)，然后提交(commit)所有暂存了的修改，如此反复。所以使用 Git 时文件的生命周期如上图。

简而言之， 当你增加一个没有进行git add的文件， 它就是untracked状态。 
而如果你修改了一个你已经跟踪（tracked）的文件， 它就会变为modified状态。 进一步， 你将这个修改过的文件通过**git add【文件名】** 加入了staging area, 这时它就可以被提交（commit）了。 
最后， 你要将这个提交， push到你的GitHub上， 用git push.

#### Checking the Status of Your Files（检查当前文件状态）
以上各种文件状态， 都是可以查看的， 用到的Git命令为：
```
$ git status
```

以我的为例

![](https://img-blog.csdnimg.cn/20190131181442954.png)

我的Git跟踪文件目前没有修改， 所以nothing to commit, working tree clean.
没有要提交的内容， working tree(工作目录)很干净。

现在我们新建一个文件， 它就是未被跟踪的（untracked）
![](https://img-blog.csdnimg.cn/20190131181810780.png)
熟悉的问题， 看来我之前出现的问题就是在这里。 我新添加的文件仅仅在我本地的工作目录上（working dictionary）， 但它要被提交到git directory才可以被Git控制。

推荐大家继续将<a href="#pic">Git的工作目录和Git的状态结合起来看。</a>
![](https://img-blog.csdnimg.cn/2019013118222919.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)
现在更加理解了， 我们工作的地方在本地文件夹， 也就是working directory. 而Git要对我们的文件夹进行监控与控制， 是在git directory,

再重新回顾一下这<a href="#concept">三个工作区域的</a>概念， 相信你会更加理解。

