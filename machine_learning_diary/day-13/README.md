# Day13：Python入门之Try/except 异常处理 

欢迎大家回到GirlsInAI👏

今天是 **[machine_learning_diary](https://github.com/YZHANG1270/Girls-In-AI/tree/master/machine_learning_diary)** 的day-13, 来带大家学习Try/except 异常处理 
<br><br>  

不知道大家还记不记得在while那一节学到的有个内容叫‘用户输入’（input()) ，今天我们就用这个讲一下异常处理  
比如下面一段代码  
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/ml_day13/1.png?raw=true" width="80%" height="80%" />   
🦁️之前告诉过你们吧，input()返回出来的是string（即使用户输入的是一个数字），所以在user_input+1这一句的时候返回错误了，一个字符串不能加一个数字。   
<br>
那我们修改一下：   
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/ml_day13/2.png?raw=true" width="100%" height="100%" />  
好，那我们想一想，如果我在这里输入的数字不是3，而是一个单词’apple’呢？？  
<br>
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/ml_day13/3.png?raw=true" width="100%" height="100%" />  
Apple这个字符串长得就不像数字😂，所以肯定不能用int（）来把它转换成整数啊。  
<br><br>  
那其实显示生活中我们真的会遇到这种用户，明明让你填写一个数字，你却填了一个汉字或者标点。  
那怎么办，如果没有今天的方法，那么用户都不知道自己错在哪里；   
但有了今天的方法之后，我们就可以提醒用户你错在哪里，应该怎么做了。   
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/ml_day13/4.png?raw=true" width="100%" height="100%" />   
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/ml_day13/5.png?raw=true" width="70%" height="70%" />   
<br>  
⚠️try里面任何一步错误，都会直接执行except  
<img src="https://github.com/yanan1995/Girls-In-AI/blob/master/others/pics/ml_day13/6.png?raw=true" width="100%" height="100%" />   
<br><br> 
## 总结一下今天要点：   
- 1. try和except是同个等级，注意对齐和缩进  
- 2. 可以把try和except直接理解成另一种形式的if else来翻译，是整个程序的保险单  
- 3. Try里任何一步错误都会直接执行except的内容，所以有时候不一定是用户输入错误，也有可能是代码本身错误  
- 4. Try和except异常处理不仅可以用于处理与用户的互动，还可以用来处理任何程序bug。应用非常广泛   
<br><br> 

## 作业  
嘻嘻嘻，比四月残忍的小狮子🦁️突然出现！！！    
我们就在上次while的作业上加一个今天学习的内容吧  
<br>  
请大家编写一个程序, 重复让用户输入数字； 直到用户输入’i wanna stop’，停止并返回之前数字的个数与总和。 如果用户输入的不是数字，使用try/except来处理异常， 并打印错信息。 然后跳过继续执行循环。   
今天就没提示啦，上次做出来的，这次应该也会啦！  
