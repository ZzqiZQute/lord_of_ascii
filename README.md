## A S C I I 之 主

![A S C I I 之 主](https://github.com/ZzqiZQute/lord_of_ascii/blob/master/lord_of_terminal.gif)

宁好，欢迎宁来前来围观:joy:,请宁先阅读以下注意事项

### 注 意 事 项

1. 宁需要在一台运行Linux内核的系统中运行这个脚本
2. 请宁安装以下程序

    1. `python3`（用于播放终端字符文件）
    2. `mpv`（用于播放音频）
3. 宁需要配置以下终端，首先它要能够显示彩色的字符，其次，它的波特率要够大，这样才不会掉帧
4. 请宁为文件夹中的`play.py`文件添加可执行权限 `chmom +x play.py`
5. 直接使用终端进入文件夹，并执行`./play.py`
6. 根据提示调整终端大小，宁可以使用ctrl+鼠标滚轮，或ctrl+加号或减号进行调整
7. __奥利给！！！__

### 原 理

[CSI转义序列 https://w.upupming.site/wiki/ANSI%E8%BD%AC%E4%B9%89%E5%BA%8F%E5%88%97#CSI%E5%BA%8F%E5%88%97](https://w.upupming.site/wiki/ANSI%E8%BD%AC%E4%B9%89%E5%BA%8F%E5%88%97#CSI%E5%BA%8F%E5%88%97)（感谢大佬的镜像地址，可以不用科学上网了:smile:)

宁可能使用过很多的终端程序，其中一部分程序的输出是彩色的，它们是怎么改变颜色的呢？

使用CSI - 控制序列导入器（Control Sequence Introducer）就可以为终端的字符进行样式修改，在终端中输出`\033[xxm`或者`\x1b[xxm`（其中`xx`是一个数字)，就能够改变当前的终端输出字符状态，为其添加颜色或者其他样式。例如
```shell
echo "\x1b[31mHello world\x1b[39m AO LI GEI"
```
上述代码输出了

![aoligei](https://github.com/ZzqiZQute/lord_of_ascii/blob/master/helloworldaoligei.png)
 

的字样

而视频转变成ASCII，目前已经有很多成熟的解决方案，_Video 2 Ascii Art_ ,blabla... 。本人之前做了一个生成这种视频的生成器[CharVideo](https://github.com/ZzqiZQute/CharVideoCharVideo),需要使用Qt和FFMpeg进行视频计算与生成。而这个时间太久了，也没有进行维护，现在基本已经废掉了(:joy:)，但是能够输出简单的视频，如果宁感兴趣也可以尝试以下。

<blockquote>
    我们遇到什么程序，都不要怕，微笑着面对它，消除bug的最好方法就是不断的写更多的新bug。坚持，才是胜利！加油，奥利给！！！------朝阳冬泳怪猿
<blockquote>

### 赠 品
1. 坤坤打篮球
2. 坏苹果
