

# Bool 布尔表达式

欢迎大家回到 **Machine Learning Diary**👏

**今天来带大家学习布尔表达式。**



简单来说，bool 就是**对错判断**。给个条件，**如果满足条件就返回True, 不满足条件就返回False。**

布尔就是BOOL的音译，如果以后看到一个数据格式叫boolean，本质上是一个判断。 

打开Jupyter，new一个python文件，输入：

```
5 == 5
```

运行后，输出：

```
True
```

再输入：

```
5 == 6
```

run一下，输出：

```
False
```



## 逻辑运算符 

就像数学有运算符号，逻辑也有运算符号，使得多个逻辑进行组合。

```
x == y
x != y 
x > y
x < y
x is y
x is not y
x and y
x or y
not (x>y)
任何数字本身，都是 True
```

可以通过下面的例子进行逻辑运算符号的熟悉：

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/bool/2.png?raw=true)

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/bool/5.png?raw=true)

   

输入：

```
x = 5 # 将x赋值为5
17 and x>4  # x>4为真True，数字17为真True，逻辑是True and True，返回为True
```

输出：

```
True
```



 ## 注意

**1. 这些符号并不是数学符号** 

比如数学里面的等号“=”, python里的等号是”==“； 
python里的“=” 是“赋值”，即我们在 **“变量”** 那一节学的内容，x=5, x作为一个变量，它的值是5

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/bool/3.png?raw=true)

**2. 布尔表达式返回的True和False，是布尔类型的两个取值，它们不是字符串string**

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_diary/bool/4.png?raw=true)

第一个是布尔表达式返回的True，不带引号；
第二个是字符串string返回的格式str (string), 带引号。
**type( )** 可以用来查询变量的格式。  



今天的内容是不是很简单呢？但不要忘了自己动手写一下哦。Coding就是熟能生巧！
