# dict 字典

欢迎大家回到 **Machine Learning Diary**~~👏

今天这节课主要带大家感受一下 dict这种数据类型。dict全称dictionary，在其他语言中也称为map，使用键-值（key: value）存储，就像查字典一样。

之前用list是中括号[]，那么在dict使用的符号就是大括号{}。所以dict的基本格式就是

**dict = {key1: value1, key2: value2, ...}** 

注意的点：

- 每个key是唯一索引，不在一个dict里重复出现
- dict是没有顺序的，不能按照位置来查找



## 新建 dict

建一个字典来记录 张三、李四、王五 三个人的数学成绩。

```python
d = {'张三': 99, '李四': 98, '王五': 66}
```



## 查找/替换 value

- 查找

```python
d['张三']    # 按照key查找对应的value
# output: 99
```

- 替换

```python
d['张三'] = 59  # 直接给key赋值，进行值的替换
d['张三']       #此时打印出来的是刚刚赋值的分数
```

- 判断字典中是否存在某key

  - 'key' in dict

  ```python
  # 比如判断下“陈二”这个人的分数在不在字典里
  '陈二' in d
  
  # output: False
  ```



  - d.get('key', 'return')
  - d.get('key')，return None

  ```python
  d.get('陈二','此人不存在')
  
  # '此人不存在'
  ```




## 添加 key-value

```python
d['陈二'] = 100    # 直接添加 陈二 和 他的分数
print(d)           # print出来的是4个人的分数

# {'李四': 98, '张三': 59, '王五': 66, '陈二': 100}
```



## 删除 key-value

```python
d.pop('李四')    # 直接用pop(key)，把这个人删除了
print(d)

# {'张三': 59, '王五': 66, '陈二': 100}
```

👩好啦，今天的课程就到这里啦！咱们下次见！~
