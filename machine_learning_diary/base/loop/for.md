# for 循环

欢迎大家回到 **Machine Learning Diary**~~👏

今天这节课主要带大家感受一下 for 循环。和while一样，for循环用来替代重复劳动力。



for循环的样子：**for ... in ...** 

来看个简单的for循环例子：

```python
for i in range(10):
    print(i)
```

run一下，output：

```
0
1
2
3
4
5
6
7
8
9
```

在 for ... in ...的in后面，跟随的是一个区间，是可以循环的内容。

所以，可以用for循环出list的内容：

```python
gia = ['girls', 'in', 'AI']
for i in gia:
    print(i)
    
# girls
# in
# AI
```

接下来，我们来用for做道题：1+2+3+...+100=？

```python
num = 0
for i in range(1,101):
    num = i + num
    
print(num)
# 5050
```



增加条件：每当10的倍数出现时，把这个数字打印出来，运行下面例子：

```python
num = 0
for i in range(1,101):
    num = i + num
    
    if i%10 == 0:  # 增加判断条件，i除以10的余数为零，即10的倍数，为True
        print(i)
    
print(num)
```



## 作业：判断谁是小偷

抓了a,b,c,d4名犯罪嫌疑人。其中有一名是小偷，审讯中：

- a说我不是小偷
- b说c是小偷
- c说小偷肯定是d
- d说c胡说！

其中有3个人说的是实话，一个人说的是假话，编程推断谁是小偷。

先尝试自己做，再跑下面的例子，看看小偷是谁。

```python
for thief in ['a','b','c','d']:
    sum = (thief != 'a') + (thief == 'c') + (thief == 'd') + (thief !='d')
    if sum == 3:
        print("小偷是：%s " % thief)
```

作业题来源：[**pythonstudy.md**](https://github.com/pythonpeixun/article/blob/master/pythonstudy.md) 

👩好啦，今天的课程就到这里啦！咱们下次见！~