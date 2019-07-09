首先表达一下对这个项目发起者的感谢！ [项目链接](https://github.com/YZHANG1270/Girls-In-AI/tree/master/machine_learning_diary/day-2)

我的个人网站[janeqinblog.com](http://janeqinblog.com/)的搭建是参考了ZHANGYI的博客[YZHANG](http://codewithzhangyi.com/2018/04/19/%E5%A6%82%E4%BD%95%E6%90%AD%E5%BB%BA%E8%87%AA%E5%B7%B1%E7%9A%84%E4%B8%AA%E4%BA%BA%E7%BD%91%E7%AB%99%EF%BC%88%E4%B8%8A%EF%BC%89/) 她同时也是项目的发起者
这篇文章将用来记录我在学习过程中遇到的问题及解决方案，希望能够帮助到和我遇到相同问题的人

###  machine_learning_diary/day-2
**issuses:**
- python3.5下载完成、 配置环境变量之后，进行到 *下载python3.5版本的 Jupyter Notebook* 这一步 出现了错误，如下图：
![error](https://img-blog.csdnimg.cn/20190114230700536.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)
socket.timeout: The read operation timed out
初步感觉是网络方面的问题， Google之后在Stack Overflow上找到了答案.
[参考链接](https://stackoverflow.com/questions/43298872/how-to-solve-readtimeouterror-httpsconnectionpoolhost-pypi-python-org-port)

![](https://img-blog.csdnimg.cn/20190114230931722.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)
**解决方案：**
依照上方提示， 打开Anaconda Prompt， 在命令行中输入：
```
pip install --default-timeout=100 jupyter notebook
```
成功解决问题

另： 可以把环境变量看成是笔记本， python3.5看做是写笔记， 买好笔记本（搭建好环境）才可以写东西。
![](https://img-blog.csdnimg.cn/20190114231609638.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)
这就是我在jupyter“笔记本”上写的笔记啦！ 哈，学习使我快落，Learning makes me happy(熬夜伤肝).

Feeling: 做的过程中会遇到非常非常多的、一个接一个的问题， 这时候要调整心态， 发现一个说明有一个提高的点， 首先接受它， 无法处理的话先记录下来， 之后通过搜索或者提问， 一步一步解决， 最后！ 就可以写成笔记和经验， 内化成你自己的小宝藏！ （仓鼠屯瓜子）我要当最胖胖的仓鼠！
