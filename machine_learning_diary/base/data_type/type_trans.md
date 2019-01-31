# 数据类型转换

欢迎大家回到 **Machine Learning Diary**~~👏

今天这节课主要带大家感受一下，数据类型是可以互相转换的。

打开jupyter，打开python。



## 数据类型回顾

前面几节课里，我们已经见过了几种常见的数据类型

- int 整数
- float 浮点数
- bool 布尔值
- string 字符串
- ...



## 转换成整数

- int( )
- round( )

输入：

```python
print(3.5/2)		# 直接除法，有小数点
print(int(3.5/2))   # 直接取整数部分
print(round(3.5/2)) # 进行四舍五入取整
print(int('4'))     # 将字符串转换成整数，字符串引号内需要本身就是整数
```

run一下，输出：

```
1.75
1
2
4	 
```

一般是浮点数转换成整数。



## 转换成浮点数

- float( )
- round( )

输入：

```python
print(4/2)                    # 答案直接是整数，只取一位小数
print(float(3.17/2))          # 答案为有限位小数，直到输出完整答案为止
print(float('3.5'))           # 将字符串转换成浮点数，字符串引号内为数字
print(round(0.123456,4))      # round可控制浮点数精度，第二个参数‘4’为保留4位小数
```

run一下，输出：

```
2.0
1.585
3.5
0.1235
```



## 转换成字符串

- str( )

输入：

```python
print(str(4.5))
print(str(5))
print(str(True))
```

run一下，输出：

```
4.5   # 这些数字已经变成字符串类型
5
True
```



## 转换成布尔值

- bool( )

输入：

```python
print(bool(10))              # 任何非零数字判断为 True
print(bool(0))               # 数字零判断为 False
print(bool(3.9))             # 非零数字判断为 True
print(bool(''))              # 空字符串判断为 False
print(bool(None))            # None 空值判断为 False
print(bool('Girls-In-AI'))   # 任何非空字符串判断为 True
```

run一下，输出：

```
True
False
True
False
False
True
```



## 检查数据类型

- type( )

有时候肉眼看着好像没变，但实际上数据类型已经变了。所以我们可以通过```type()``` 来检查一下。

输入：

```python
a = str(False)  # 将bool值转换成字符串，并赋值给变量 a
print(bool(a))  # a 为非空字符串，用bool转换后，判断为 True
```

run一下，输出：

```
True
```



👩好啦，今天的课程就到这里啦！咱们下次见！~