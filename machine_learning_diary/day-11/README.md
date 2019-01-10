
# Day11：Python入门之while语句

欢迎大家回到GirlsInAI👏

今天是 **[machine_learning_diary](https://github.com/YZHANG1270/Girls-In-AI/tree/master/machine_learning_diary)** 的day-11, 来带大家学习while语句,并不难哦，只是需要认真！

学习内容 
- 新值替换变量  
- 一般while语句 
- 无限循环 & break  
- continue  
- 作业  

## 更新变量  
开始之前，有个小要点大家可以掌握一下（对今天的练习题有帮助哦）  
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/ml_day11/1.png?raw=true" width="90%" height="90%" />  
<br>
## 一般while语句  
大家做重复性工作的时候都会觉得很麻烦，浪费时间，浪费生命，这时候计算机就登场了。  
计算机可以执行很多重复性的任务，python也有一些特定语句来执行这些任务。   
其中常见的一种就是while  
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/ml_day11/2.png?raw=true" width="90%" height="90%" />  
当然，这些判断条件，包括满足条件/退出迭代之后的动作，你们都可以自己决定，我这里就直接用print(’n’) & print(‘end’)来表示  
因为n在每次一循环的时候，值都会改变，所以被称为“迭代变量”；  
如果没有迭代变量，循环会永远进行下去，导致无限循环。   
<br>  
## 无限循环 & break    
我们来看一下无限循环的例子和怎么打断无限循环。  
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/ml_day11/3.png?raw=true" width="60%" height="60%" />  
那怎么打断这种无限循环呢？ 用break   
Break就是打断，破坏的意思  
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/ml_day11/4.png?raw=true" width="90%" height="90%" />   
图片里面体现不出来（可以自己敲一下代码），上面返回的四句话，只有第一句和第三句是我自己输入的，第二句和第四句是它自动返回的（我们刚刚的代码）  
⚠️ input()这个返回的数据格式都是字符串，尽管你可能输入的是一个数字  
<br>   
## continue  
还有一种情况，如果在循环中，你想结束当前的迭代，立刻进行下一次迭代，那么就可以用continue （而不用完成当前迭代）   
什么意思呢？  
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/ml_day11/4.png?raw=true" width="80%" height="80%" />  
其中第一行/第二行/第四行/第五行是我输入的，其它是自动返回的  
<br>
我们来理一下这个顺序和逻辑  
当我第一次输入‘#how are you’的时候，第一个条件被满足，然后continue，进行下一次循环，再从while true开始  
然后输入第二句话’good’， 第一个条件不满足，第二个条件也不被满足，所以print这句话，所以出现两个good   
然后输入第三句话’#fine’，同第一次输入一样，continue，进行下一次循环，再从while true开始  
然后第四句话’I wanna stop’，不满足第一个条件，满足第二个条件，所以break,然后最后print(‘we can stop now’)   
<br>
## 作业
嘻嘻嘻，比四月残忍的小狮子🦁️突然出现！！！  
今天是有小练习的哦，我的例子看起来简单，但需要举一反三的有很多内容哦！！！  
请大家编写一个程序, 重复让用户输入数字； 直到用户输入’i wanna stop’，停止并返回之前数字的个数与总和。   
<br>  
🦁️提示：   
重复 —— while   
让用户输入 —— input()  
直到 —— break   
个数与总和 —— 需要用到我们最开始的内容 “用新值替换变量”  


