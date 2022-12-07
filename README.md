# 我的Python学习 #

## Linux常用命令 ##
|命令			|作用						|使用										|
|---			|---						|---										|
|cd				|切换文件目录					|cd 目录（切换到目录）；cd ..（返回上级目录）；	|
|ls				|列出目录下的文件夹与文件		|ls											|
|mkdir			|创建文件夹					|mkdir Py-study（创建一个叫Py-study的文件夹）	|
|touch			|创建文本文件					|touch README.md（创建README.md文件）			|
|pwd			|打印当前文件夹路径			|pwd										|
|rm				|删除指定文件名				|rm -d 目录(删除目录）；rm 文件（删除文件）	|
|clear			|清除终端					|clear										|
|exit			|退出终端连接					|exit										|
|command --help	|显示command命令帮助信息		|git --help									|
|man command	|查询command命令的使用手册	|man git									|
|cp				|							|											|

### man command ###

使用man时操作键：

|操作键	|功能				|
|---	|---				|
|空格键	|显示手册页的下一屏	|
|Enter键	|一次滚动手册页的一行	|
|b		|回滚一屏			|
|f		|前滚一屏			|
|q		|退出				|
|/word	|搜索word字符串		|

### ls命令说明 ###
**Linux下文件和目录特点**

- Linux文件或者目录名称最长可以有**256**个字符
- 以<kbd>**.**</kbd>开头的文件为隐藏文件，需要调用-a参数才能显示
- <kbd>.</kbd>代表当前目录
- <kbd>..</kbd>代表上一级目录

**ls常用选项**

|参数	|含义										|
|---	|---										|
|-a		|显示指定目录下所有子目录与文件，包括隐藏文件	|
|-l		|以列表方式显示文件的详细信息					|
|-h		|配合-l以拟人化的方式显示文件大小				|

**ls通配符的使用**

|通配符	|含义							|用法										|
|---	|---							|---										|
|\*		|代表任意个数个字符				|ls \*1.txt（列出所有以1.txt结尾的文件）		|
|？		|代表任意一个字符，至少一个		|ls 1?1.txt（列出所有1?1.txt文件）			|
|[]		|表示可以匹配字符组中的任意一一个	|ls [123]12.txt（列出112，212，312.txt文件）	|
|[abc]	|匹配a、b、c中任意一个				|ls [123]12.txt（列出112，212，312.txt文件）	|
|[a-f]	|匹配从a到f范围内的任意一字符		|ls [1-3]12.txt（列出112，212，312.txt文件)	|

### cd命令说明 ###
- <kbd>cd</kbd>是英文**change directory**的简写，其功能为更改当前的工作目录，也是用户最常用的命令之一。

> 注意：Linux所有的目录和文件名都是大小写敏感的

|命令	|含义									|
|---	|---									|
|cd		|切换到当前用户的主目录（/home/用户目录）	|
|cd ~	|切换到当前用户的主目录（/home/用户目录）	|
|cd .	|保持在当前目录不变						|
|cd ..	|切换到上级目录							|
|cd -	|在最近两次工作目录之间来回切换			|

### 相对路径和绝对路径 ###
- **相对路径**：在输入路径时，最前面没有<kbd>/或者~</kbd>，表示相对**当前目录**所在的目录位置
- **绝对路径**：在输入路径时，最前面的是<KBD>/或者~</kbd>，表示从**根目录/家目录**开始的具体目录位置

