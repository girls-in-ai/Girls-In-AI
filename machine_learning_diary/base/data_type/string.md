
# String 字符串

欢迎大家回到 **Machine Learning Diary**👏

今天来带大家学习字符串。

- 字符串的性质  
- 字符串的玩法




## 字符串的性质  
字符串用引号表示 例如’water’ 。

#### **字符串就是字符的序列**

我们说的是序列，那就代表字符串是有顺序的！这里很重要。比如我们来设定一个变量phone，给它赋值一个‘apple’
![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/string/1.png?raw=true)

#### **字符串不可改变**

即字符串里的每一个字符都不可以被替代
![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/string/2.png?raw=true)




## 字符串的玩法  
#### len( ) 

返回字符串的长度，即字符串有多少个字符

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/string/3.png?raw=true)

‘apple’这个字符串一共有5个字符，’a’, ‘p’, ‘p’, ‘l’, ‘e’

我们可以在这个函数上加一些玩法

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/string/4.png?raw=true)



#### 分割字符串 

利用‘找字符’的方法‘[ ]’ 我们不仅可以找单独一个字符，我们也可以提取‘一部分’的字符串

例如我们想提取’apple’里面的最后三个字符’ple’

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/string/5.png?raw=true)

- 你们看是不是有点奇怪，为什么我提取e的时候用的是length, 而不是length -1？  

  分割字符串的时候冒号‘:’只包括第一个字符，而不包括最后一个字符，所以为了提取出最后一个，我们要比平常的索引多一位！

- 一些可以注意的例子
  ![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/string/6.png?raw=true)



#### 用 `in` 找字符 

in 是一个布尔运算符，可以比较两个字符串，所以返回值是true/false,很好理解，如 
<img src="https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/string/7.png?raw=true" width="50%" height="50%" />  



#### 其它方法method 

这里叫方法method，而不是函数function，但都是进行操作。区别是method是使用句点作为分割，在变量名后跟上方法名，而不是在函数function括号里面加上变量名。对比一下：
len(phone) — function 
phone.upper() — method   



- upper/lower/find/strip/startswith 
  <img src="https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/string/8.png?raw=true" width="80%" height="80%" />   
- string.split(seperator, maxsplit) 字符串的切割 
  这个方法和字符串的分割用[ ]和冒号：类似。
  <img src="https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/string/9.png?raw=true" width="80%" height="80%" />  
- Split的反义词join, 同义就是把分割开的东西连起来 
  <img src="https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/string/10.png?raw=true" width="80%" height="80%" />  



#### 格式操作符

用百分号%表示，简单来说，就是用其它变量来替代某字符串的一部分 
看一个例子就懂了 
<img src="https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/string/11.png?raw=true" width="50%" height="50%" />  

对于下面一个例子而言，我有多少个苹果这个‘多少个’是可以随时切换随时被替代的，那我就用格式操作符号来表示。 一个完整的例子需要两个格式操作符，一个在字符串里（后面紧跟格式！待会讲），一个在字符串外（后面跟变量）  

第一个字符串紧跟的格式是固定的

- %d —— 格式化整数
- %g—— 格式化浮点数（带小数部分）
- %s —— 格式化字符串
  
  <img src="https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/string/12.png?raw=true" width="80%" height="80%" />  

- 百分号%对int这个数据格式而言，是模运算符； 但对字符串而言，%是格式操作符  

这样的函数和方法还有很多，运用起来并不困难。 没用过或者没见过这些函数都没关系，只要你在实践操作中遇到这样的难题，然后在网上直接搜索相关用法，就可以得到答案了。
还是那句话，熟能生巧。 你遇到的问题，别人早就遇到过了。 
