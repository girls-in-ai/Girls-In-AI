# Day5：数据类型

欢迎大家回到GirlsInAI~~👏

今天是machine_learning_diary的day-5，这节课主要带大家熟悉一下计算时将会碰到的各种数据类型。

打开jupyter，new一个新python文件。



## 数字

最常见的计算就是数字与数字之间的计算了，在python里，数字大致可以分为两种：

- 整数 int
- 小数（浮点数）float

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day5/001.png?raw=true)

大家可以参照上面图片的计算公式随便尝试，python的计算都是非常直观的，与常识相符。



## 文字

能计算的不只是数字，文字也可以进行计算。文字在代码里的称号叫做“字符串”，由英文单词“string”而来。一起来看看文字是如何进行计算的吧！

#### 字符串 string

文字的出现是必须随身带引号的```'单引号' ，"双引号"``` ，单双引号都可以，只要是英文格式的。这里举个字符相加的例子：

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day5/002.png?raw=true)

谨记，使用字符串时，一定带上引号，否则只能做变量处理。当你直接输入字符却不带引号时，会报错。把引号加上去，就不会了。

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day5/003.png?raw=true)



#### 转义字符

如果是字符串里面需要包含单双引号怎么办，比如```I'm a GIAer``` 这个句子里就有个单引号。这里可以用转义字符```\``` 来标识。

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day5/004.png?raw=true)

第一句里面没有使用转义字符```\``` 就会报错。第二局加上就ok了~

转义字符还有很多其他表示：

- ```\n``` 表示换行
- ```\t``` 表示tab
- ```\\``` 表示```\``` 斜杠本身

请尝试用python的print打出这两句话：

`I'm a GIAer.`

`I'm learning machine learning by 'python'`

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day5/005.png?raw=true)



## 判断逻辑

#### 布尔值 bool

这里还有种数据是用来做逻辑判断的，叫做布尔值，根据英文名而来。

布尔值有两种数值：

- True
- False

在python里可以直接输入做计算，也可以用```and``` ，```or``` 等做运算。后面的课程还会有详细介绍。

![](https://github.com/YZHANG1270/Girls-In-AI/blob/master/others/pics/ml_day5/006.png?raw=true)



## 空值

空值代表这个值存在，但是不知道这个值是什么，一般用```None``` 表示。



## 变量

变量是一个可以随意赋值的值。



## 常量

常量是一个固定值的值。



这里只做简单的介绍，其他的数据类型还有list，dict等等，后面还有更多有趣的小例子来深入了解各种类型的数据。

👩好啦，今天的课程就到这里啦！咱们下次见！~