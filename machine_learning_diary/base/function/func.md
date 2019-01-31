# function 函数

欢迎大家回到 **Machine Learning Diary**~~👏

今天这节课主要带大家感受一下function函数。函数相当于一个固定的公式，一个映射。有输入，有输出。



## python内置函数

首先python内部有很多好用的内置函数，有些我们已经使用过了。

- max()   求最大值

- min()    求最小值

- abs()     求绝对值

- int()       转换成整数

- range()  返回一个区间
- ...

可以尝试下面的例子：

```python
print(max(1,2,3,4))
print(max([1,2,3,4]))  # max() 里面可以是一串数字，也可以是一个list

print(abs(-1.23))
print(list(range(5)))
```



## 自定义函数

我们来自定义一个加法的函数：

```python
def add(x,y):   # add为函数名，x,y为参数
    return x+y  # x+y 为映射关系

add(4,100)  # 调用函数
# 104
```

所以一个自定义函数的元素有：

- def 开头
- 函数名
- 是否有参数，如果有，参数是什么
- 映射关系是什么
- 如果有返回结果，请输出结果



再写一个没有参数的函数：

```python
def sayHi():  # 没有参数，直接为空
    return 'hello, girls in AI!'

sayHi()  # 调用函数
```



## 调用函数

函数名+括号，括号内填参数

直接返回结果



## 作业

制作一个包含for，if的函数

举例：

```python
def GIA(heart):  # 这个heart是参数，是一个字符串的参数
    print('\n'.join([''.join([(heart[(x-y)%len(heart)]if((x*0.05)**2+(y*0.1)**2-1)**3-(x*0.05)**2*(y*0.1)**3<=0 else' ')for x in range(-30,30)])for y in range(15,-15,-1)]))

GIA('GirlsRunTheWorld') # 我把heart赋值为 'GirlsRunTheWorld'
                        # 赋值时，请记得加引号
```

output：

```
                                                          
                                                            
                unTheWorl           eWorldGir               
            lsRunTheWorldGirl   nTheWorldGirlsRun           
          rlsRunTheWorldGirlsRunTheWorldGirlsRunThe         
         rlsRunTheWorldGirlsRunTheWorldGirlsRunTheWo        
        rlsRunTheWorldGirlsRunTheWorldGirlsRunTheWorl       
        lsRunTheWorldGirlsRunTheWorldGirlsRunTheWorld       
        sRunTheWorldGirlsRunTheWorldGirlsRunTheWorldG       
        RunTheWorldGirlsRunTheWorldGirlsRunTheWorldGi       
        unTheWorldGirlsRunTheWorldGirlsRunTheWorldGir       
        nTheWorldGirlsRunTheWorldGirlsRunTheWorldGirl       
         heWorldGirlsRunTheWorldGirlsRunTheWorldGirl        
          WorldGirlsRunTheWorldGirlsRunTheWorldGirl         
          orldGirlsRunTheWorldGirlsRunTheWorldGirls         
            dGirlsRunTheWorldGirlsRunTheWorldGirl           
             irlsRunTheWorldGirlsRunTheWorldGirl            
              lsRunTheWorldGirlsRunTheWorldGirl             
                unTheWorldGirlsRunTheWorldGir               
                  heWorldGirlsRunTheWorldGi                 
                    orldGirlsRunTheWorldG                   
                       GirlsRunTheWorl                      
                          sRunTheWo                         
                             The                            
                              e                          
```

👩好啦，今天的课程就到这里啦！咱们下次见！~

