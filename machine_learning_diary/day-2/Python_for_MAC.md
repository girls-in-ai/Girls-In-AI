# Python 环境配置 Mac版本

下载3.5 version:

[下载地址]: https://www.python.org/ftp/python/3.5.2/python-3.5.2-macosx10.6.pkg

双击下载好的安装包，然后无脑下一步就安装好了。

然后应用列表里找到一个叫“终端”的黑黢黢的软件。

![terminal_screen_shot](https://raw.githubusercontent.com/ohdroid/Girls-In-AI/973d3c380a3eaa0b2402af18dcb790359dc1f575/others/pics/ml_day2_mac_os/terminal_screen_shot.png)

打开后类似长这样

![image-20190112140157064](https://github.com/ohdroid/Girls-In-AI/blob/master/others/pics/ml_day2_mac_os/screen_shot_for_terminal.png?raw=true)

由于是个花里胡哨的程序员，所以这个界面颜色你们的有点不一样，功能是一致的。

然后关键和重点来了，这里有个超级关键的武功秘籍，所有程序员必须掌握的。

让电脑执行我们想要的功能，一般有两种主流方式：1.通过图形化的操作界面进行操作（就是类似微信和网易云音乐一样的软件），这种方式就是那里执行点哪里。2.程序员的我们当然是用非主流装X成风的方式，就是打字给电脑，让电脑做我们想要功能，就好像和电脑是用文字交流的。所以我们在终端软件里输入特定的字符来和电脑交流。

下面就操作一下，输入特定字符，让电脑告诉我们刚刚的python3.5 是否安装好了.

![check_python3.5](https://raw.githubusercontent.com/ohdroid/Girls-In-AI/master/others/pics/ml_day2_mac_os/check_python3.5.GIF)

这里有个小技巧，就是python命令不用完全一个一个字符打完全，像程序猿这种懒癌晚期的，肯定想了有千奇百怪的偷懒方式，当输入pyth后，双击键盘上的Tap键，奇迹就发生了自动补全了。你也看到我电脑上装了好几个版本的python，所以这里我们需要选择对应的版本执行对应的操作，python3是我这台电脑上对应的python3.5，输入python3后回车，就进入python3.5的程序了，上面内容也能看到，输入exit()后回车是退出python3.5程序。

接下来通过python去安装jupyter软件，使用命令行的方式和电脑沟通是非常高效快捷的，多接触你会爱上这样的方式（装起X来别个都看不懂）。 

安装步骤：

1.确认使用python3.5 对应的pip：pip3 --version

2.通过pip命令安装jupyter：pip3 install jupyter

3.等待下载完成OK就可以了。

```shell
#注：如果遇到SSL的异常，可以输入以下命令修正，没有遇到就忽略就好
curl https://bootstrap.pypa.io/get-pip.py | python3
```

操作的gif图如下。

![pip_install_jupyter](https://raw.githubusercontent.com/ohdroid/Girls-In-AI/973d3c380a3eaa0b2402af18dcb790359dc1f575/others/pics/ml_day2_mac_os/pip_install_jupyter.gif)

安装好过后，需要让终端认识jupyter命令(这个就相当于教狗子握手🤝的过程)

这里需要配置个环境变量，可以让终端认识jupyter这个命令，步骤如下

1.找到jupyter的安装位置：pip3 show jupyter

2.拷贝位置（框中文字后，键盘上Command + C组合键进行复制）

3.打开环境变量配置文件：open ~/.bash_profile

4.键入以下内容：export PIP_INSTALL_PATH=jupyter_location(把这个jupyter_location用复制的安装路径覆盖)

5.应用环境配置文件：source ~/.bash_profile

6.关闭终端，重新打开使配置生效

7.终端中键入：jupyter --version

老年人手法下的操作流程GIF图

![add_jupyter_to_bash_path](https://raw.githubusercontent.com/ohdroid/Girls-In-AI/973d3c380a3eaa0b2402af18dcb790359dc1f575/others/pics/ml_day2_mac_os/add_jupyter_to_bash_path.gif)

好的就酱紫完成了。有任何问题都可以在issue中回复