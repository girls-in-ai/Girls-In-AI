# GitHub-Issue 正确的提问方式

> 对开源项目来讲，问题追踪是很重要的。在整个GitHub，谁都可以提问issue，谁都可以对issue问题进行回答。但如果没有适当的处理，项目会变得很庞大，挤满重复的bug issue、模糊不明的feature request。项目维护者会被大量工作压得喘不过气来，新的贡献者也搞不清楚项目当前的工作重点是什么。接下来，我们一起研究下，如何玩转 GitHub 的issue。



## Issue 礼仪

提问是需要有礼仪的。

1. **提问使用的语言** ：第一，参照维护者的母语，比如GIA维护者的母语就是中文。第二，一般可选择英文。
2. **提问态度和语气** ：因为你是面向整个GitHub用户提问，不卑不亢，虚心求教就可以了，不必要太咋呼。
3. **如有issue模板，请参照模板写issue**



## Templates for GIA 模板

> 统一的问题单模板可以大大减轻项目维护者的负担，尤其是开源项目的维护者。

目前我创建了两类模板：Bug report 和 Feature request。模板的核心点在于，问题单要清晰的呈现给它涉及的每一个人：它要尽量简单的指明受众（或者说用户），操作（或者说任务），和输出（或者说目标）。不过，不需要过分拘泥于这个模板，只要能把事情说清楚就好了。



### 模板1. Bug report：描述你在学习中遇到的问题

**为避免无效问题和冗余问题，提问前请确认**

1. 你确定Google不能解决你的问题
2. 你确定已有的issue不能解决你的问题
3. 你确定issue的title按照格式如下：[tutorial-code]：description

**Describe the bug 描述你遇到的问题**
A clear and concise description of what the bug is. 简洁有效的说明。

**To Reproduce 如何重现问题**
Steps to reproduce the behavior: 把你遇到的问题的发生步骤替换掉下面的内容：

1. Go to '...'
2. Click on '....'
3. Scroll down to '....'
4. See error

**Expected behavior 期待修复的效果**
A clear and concise description of what you expected to happen. 简单描述。

**Screenshots 如有必要，可以截图说明**
If applicable, add screenshots to help explain your problem.

**环境版本说明**

- OS: [e.g. win] 说明操作系统
- Python Version 说明语言及版本号
- Package Version 相关库/包的版本
- Browser [e.g. chrome, safari] 如果有必要，说明浏览器型号

**Additional context 其他说明**
Add any other context about the problem here. 添加你认为有必要的内容，否则不写。



### 模板2. Feature request：帮助维护教程的有效性

**Is your feature request related to a problem? Please describe. 描述对应的教程内容**
A clear and concise description of what the problem is. Ex. I'm always frustrated when [...]
简洁有效的描述教程内出现的漏洞，或者对于教程你想做补充的地方。

**Describe the solution you'd like 说出你的解决建议**
A clear and concise description of what you want to happen. 描述你想实现的内容。

**Describe alternatives you've considered 如果你有其他想法，可以在此补充**
A clear and concise description of any alternative solutions or features you've considered.

**Additional context 其他内容**
Add any other context or screenshots about the feature request here. 添加你认为有必要的内容，否则不写。



## 一个好问题的标准

1. 避免使用术语或晦涩的文字
2. 问题可以切分，也就是说可以逐步解决的问题
3. 尽量跟其他问题没有瓜葛，依赖其它问题会降低处理的灵活性
4. 可以协商，也就说我们有好几种办法达到目标
5. 问题足够小，可以非常容易的评估出所需时间和资源
6. 可衡量，我们可以对结果进行测试



## Labels 标签

> 高质量的issue是项目成功的关键。有些人把issue仅仅看作是一堆你不得不去处理的问题列表，但是如果这些问题单管理完善，进行了分类并打上标签，会令人意想不到的提升我们对代码和社区的了解程度，也让我们更清楚问题的关键点在哪里。

每次提issue的时候，写完问题，你还可以对这个问题进行打标签。[打开Girls-In-AI项目的issue](https://github.com/YZHANG1270/Girls-In-AI/issues)，你可以看到：

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/tools/github/issue/001.png?raw=true)



1. 点击Issue
2. 点击Labels
3. 第三个框是我刚提的issue

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/tools/github/issue/002.png?raw=true)

可以看见左边一列的labels，下面红色的label是我刚刚为【Machine-Learning-Diary】建的，以后跟这个项目相关的issue可以打上这个标签，方便查找。当然后续还会继续增加合适的label。



## Issue Title 格式规范

格式：英文中括号 + 课程代码 + title描述

实例：[ml-day-1] About Jupyter Notebook Version

目前的课程代码 tutorial-code

- [ml-day-x] = Machine-Learning-Diary
- [github] = GitHub 相关使用教程
- ......
- 未完待续



## Make Issue Steps 提问步骤

初步了解issue后，下面介绍如何提issue。首先你要确认你的问题Google无法解答，因为Google还是作为首推的解答平台。

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/tools/github/issue/003.png?raw=true)

1. 点击issue
2. 查看历史上的issue能否解决你的问题，进行issue搜索
3. 确认已有issue无法解决你的问题，点击 New issue，创建新issue

接下来你将看见我在上面提到过的模板：

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/tools/github/issue/004.png?raw=true)

你要明确你是在学习过程中遇到了问题，还是觉得对于教程的内容想做贡献。在这里假设你是在学习过程中遇到了bug，点击【Bug report】的【Get started】，你将看到：



![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/tools/github/issue/005.png?raw=true)

1. 填写issue的title，title格式请按照：[tutorial-code] description

   [ml-day-1]就是Machine-Learning-Diary第一天的课程的代号，英文中括号括起来。后面写上issue的主要描述，几个字就OK。关于issue，看多了就容易写了。

2. 当你一边打title时，一边下方会出现与你的issue相关的问题。第二次确认是否已存在的issue不能解决你的问题。如果已经存在相似问题，建议去到那个问题下面进行答案搜索。冗余重复的问题对整个项目和学习者都是不利的。

3. 如果你的是个新问题，在3号框下按照模板的要求，一步步写清问题描述。用你的文字把模板文字覆盖掉。

4. 写完可以点击Preview进行预览

5. 可以到右侧的label为你的issue打一个标签

6. 提交你的issue



## Answer Issue Steps 回答步骤

每个人不仅仅可以提问，还可以回答他人的问题。

> “关注社区的成长，不仅要关注参与开发者的的数量增长，也要关注那些在issue上帮助我们的人，他们让issue更加明确、保持更新，这是活跃沟通和高效解决问题的力量源泉。”

很多人想参与/贡献到GIA这个项目里来，如果你愿意积极解决issue，也是一个很大的贡献。我也会不定期的把这些活跃的回答者揪出来好好表扬😜

那么如何在issue上贡献呢：

0. 在issue模块揪出你感兴趣的issue打开，我这里以我的测试issue为例
1. 可以用quote reply的方式，就像微博的转发。如果提问内容较长就不太建议了
2. 或者可以用艾特@的方式，就像微博的留言
3. 在框内填写你的答案
4. Comment提交

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/tools/github/issue/006.png?raw=true)

GitHub于我而言是个很神圣的地方。而且GitHub还有很多礼仪需要学习，我们下次再见~

