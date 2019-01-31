# list 列表

欢迎大家回到 **Machine Learning Diary**~~👏

今天这节课主要带大家感受一下 list这种数据类型。list是一种有序的集合，可以随时添加和删除其中的元素。

打开jupyter。



## 按顺序计数时，是从0开始计数

input:

```python
print(list(range(10)))    # range表示一个区间，数字10表示输出10个数字
print(list(range(1,10)))  # (1,10)表示输出第2个数到第10个数
```

因为python的计数是从0开始的。所以让计算机数10个数的结果就是从0到9。

output:

```python
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
[1, 2, 3, 4, 5, 6, 7, 8, 9]
```



可以从字符串转换成列表，字符串的每一个字母都成为一个单独的元素。

input:

```python
list('GirlsInAI')
```

output:

```
['G', 'i', 'r', 'l', 's', 'I', 'n', 'A', 'I']
```



## 组成元素

列表的组成元素可以由很多种，甚至一个列表内都可以有很多数据类型：

- [1, 2, 3, 4, 5]
- [True, False, True]
- ['girls', 'in', 'AI']
- ['Girls', 'run', True, 100, 7.21]

以上这些，都是列表。



## 访问元素

列表既然是有顺序的，就可以根据元素的位置进行访问。

首先可以获取列表内总共有几个元素

- len( )

input:

```python
a = ['Girls', 'In', 'AI']
len(a)
# output:3
```

那么来访问列表a的各个元素：

```python
print(a[0]) # 数字0表示访问第一位置的元素
print(a[1]) # 数字0表示访问第二位置的元素
print(a[2]) # 数字0表示访问第三位置的元素

# output:
# Girls
# In
# AI
```

注意位置数字不要超过len-1

```python
# 一共只有3个位置，如果输入 print(a[3])就会报错
print(a[3])
```

同理可以倒着来访问：

```python
print(a[-1]) # 数字-1表示访问倒数第一位置的元素
print(a[-2]) # 数字-2表示访问倒数第二位置的元素
print(a[-3]) # 数字-3表示访问倒数第三位置的元素

# output:
# AI
# In
# Girls
```

 同理也可以访问一个区间：

```python
print(a[:])   # 冒号表示一个切片，两端不填数字表示全部都要
print(a[1:])  # 左端1表示从第二个元素开始取
print(a[:-2]) # 右端-2表示取到倒数第三个元素停止

# ['Girls', 'In', 'AI']
# ['In', 'AI']
# ['Girls']
```



## 修改元素

直接给元素赋值，尝试下面例子：

```python
a[0] = 'Boys'
print(a)
# ['Boys', 'In', 'AI']
```



## 添加元素

```python
a.append('and') # append直接在list最后继续添加元素
print(a)

a.insert(1,'and Girls') # insert在指定位置添加元素
print(a)

# ['Boys', 'In', 'AI', 'and']
# ['Boys', 'and Girls', 'In', 'AI', 'and']
```



## 删除元素

```python
a.pop()   # pop直接删除最后一个元素
print(a)

a.pop(0)  # pop也可以指定元素位置，数字0为第一个元素
print(a)

# ['Boys', 'and Girls', 'In', 'AI']
# ['and Girls', 'In', 'AI']
```

👩好啦，今天的课程就到这里啦！咱们下次见！~