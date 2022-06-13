

# linux 基础

## 开关机

shutdown

shutdown -h now : 表示立即关机

shutdown -h 1 : 表示 1 分钟后关机

shutdown -r now: 立即重启

syn ： 把内存的数据同步到磁盘



## 帮助

help

man



## 3文件系统

### 文件树

![image-20200820210646213](https://gitee.com/sxy22/note_images/raw/master/image-20200820210646213.png)



![](https://gitee.com/sxy22/note_images/raw/master/image-20200820210658282.png)

![image-20200820210727040](https://gitee.com/sxy22/note_images/raw/master/image-20200820210727040.png)

![image-20200820210743259](https://gitee.com/sxy22/note_images/raw/master/image-20200820210743259.png)

![image-20200820210753792](https://gitee.com/sxy22/note_images/raw/master/image-20200820210753792.png)









## 4操作系统

### 长格式输出

![image-20210320231905658](https://gitee.com/sxy22/note_images/raw/master/image-20210320231905658.png)

### ls

![image-20210426163212903](https://gitee.com/sxy22/note_images/raw/master/image-20210426163212903.png)

### less

![image-20210320232058228](https://gitee.com/sxy22/note_images/raw/master/image-20210320232058228.png)

![image-20210320232108425](https://gitee.com/sxy22/note_images/raw/master/image-20210320232108425.png)

## 5操作文件和目录

### 通配符

![image-20210321212640204](https://gitee.com/sxy22/note_images/raw/master/image-20210321212640204.png)

### mkdir - 创建目录

mkdir  [选项]  要创建的目录

-p ：创建多级目录



### cp - 复制文件和目录

![image-20210321212852555](https://gitee.com/sxy22/note_images/raw/master/image-20210321212852555.png)

![image-20210426164150579](https://gitee.com/sxy22/note_images/raw/master/image-20210426164150579.png)

### mv - 移动和重命名文件



![image-20210321212940112](https://gitee.com/sxy22/note_images/raw/master/image-20210321212940112.png)

![image-20210321213003205](https://gitee.com/sxy22/note_images/raw/master/image-20210321213003205.png)

![image-20210321213114366](https://gitee.com/sxy22/note_images/raw/master/image-20210321213114366.png)



### rm - 删除文件和目录

![image-20210321213207686](https://gitee.com/sxy22/note_images/raw/master/image-20210321213207686.png)

### ln —创建链接

![image-20210321213345828](https://gitee.com/sxy22/note_images/raw/master/image-20210321213345828.png)

![image-20210321213516654](https://gitee.com/sxy22/note_images/raw/master/image-20210321213516654.png)

## 6使用命令

![image-20210426164823297](https://gitee.com/sxy22/note_images/raw/master/image-20210426164823297.png)

### type －显示命令的类型

![image-20210426164838876](https://gitee.com/sxy22/note_images/raw/master/image-20210426164838876.png)

### which －显示一个可执行程序的位置

![image-20210426164939827](https://gitee.com/sxy22/note_images/raw/master/image-20210426164939827.png)



### help －得到shell 内建命令的帮助文档

![image-20210426165216773](https://gitee.com/sxy22/note_images/raw/master/image-20210426165216773.png)

### --help - 显示用法信息

### man －显示程序手册页

![image-20210426165354742](https://gitee.com/sxy22/note_images/raw/master/image-20210426165354742.png)

### 用别名（alias）创建你自己的命令

![image-20210426165543852](https://gitee.com/sxy22/note_images/raw/master/image-20210426165543852.png)

![image-20210426165553135](https://gitee.com/sxy22/note_images/raw/master/image-20210426165553135.png)

![image-20210426165620677](https://gitee.com/sxy22/note_images/raw/master/image-20210426165620677.png)

## 7重定向

### 标准输入、输出和错误

![image-20210322220812622](https://gitee.com/sxy22/note_images/raw/master/image-20210322220812622.png)

### 标准输出重定向



![image-20210322220932449](https://gitee.com/sxy22/note_images/raw/master/image-20210322220932449.png)

![image-20210322221043823](https://gitee.com/sxy22/note_images/raw/master/image-20210322221043823.png)

### 标准错误重定向

![image-20210322221132743](https://gitee.com/sxy22/note_images/raw/master/image-20210322221132743.png)

### 重定向标准输出和错误到同一个文件

![image-20210427173338768](https://gitee.com/sxy22/note_images/raw/master/image-20210427173338768.png)

### cat

![image-20210322221530501](https://gitee.com/sxy22/note_images/raw/master/image-20210322221530501.png)

### 管道符 | 

![image-20210322221603637](https://gitee.com/sxy22/note_images/raw/master/image-20210322221603637.png)

### uniq - 报道或忽略重复行

![image-20210322221841445](https://gitee.com/sxy22/note_images/raw/master/image-20210322221841445.png)



### wc －打印行数、字数和字节数

![image-20220515112837025](https://gitee.com/sxy22/note_images/raw/master/img/image-20220515112837025.png)





### grep －打印匹配行

![image-20210322222011935](https://gitee.com/sxy22/note_images/raw/master/image-20210322222011935.png)



### head / tail －打印文件开头部分/结尾部分

![image-20210322222130053](https://gitee.com/sxy22/note_images/raw/master/image-20210322222130053.png)

![image-20210322222137675](https://gitee.com/sxy22/note_images/raw/master/image-20210322222137675.png)

## 8从shell 眼中看世界

### 算术表达式展开

![image-20210430203759706](https://gitee.com/sxy22/note_images/raw/master/image-20210430203759706.png)

![image-20210430203846585](https://gitee.com/sxy22/note_images/raw/master/image-20210430203846585.png)

### 花括号展开

![image-20210430204140310](https://gitee.com/sxy22/note_images/raw/master/image-20210430204140310.png)

![image-20210430204155933](https://gitee.com/sxy22/note_images/raw/master/image-20210430204155933.png)



### 命令替换

![image-20210430204607317](https://gitee.com/sxy22/note_images/raw/master/image-20210430204607317.png)

![image-20210430204634371](https://gitee.com/sxy22/note_images/raw/master/image-20210430204634371.png)

### 双引号

![image-20210430204918846](https://gitee.com/sxy22/note_images/raw/master/image-20210430204918846.png)

### 单引号

![image-20210501204056020](https://gitee.com/sxy22/note_images/raw/master/image-20210501204056020.png)





### 转义字符

![image-20210501204127281](https://gitee.com/sxy22/note_images/raw/master/image-20210501204127281.png)



## 9键盘高级操作技巧

### 光标移动

![image-20220516132445452](https://gitee.com/sxy22/note_images/raw/master/img/image-20220516132445452.png)

![image-20220516132454238](https://gitee.com/sxy22/note_images/raw/master/img/image-20220516132454238.png)

### 历史命令





## 10权限

![image-20210503163324183](https://gitee.com/sxy22/note_images/raw/master/image-20210503163324183.png)

### 读取、写入和执行

![image-20210503163440231](https://gitee.com/sxy22/note_images/raw/master/image-20210503163440231.png)

![image-20210503163506666](https://gitee.com/sxy22/note_images/raw/master/image-20210503163506666.png)

![image-20210503163526957](https://gitee.com/sxy22/note_images/raw/master/image-20210503163526957.png)

![image-20210503163533120](https://gitee.com/sxy22/note_images/raw/master/image-20210503163533120.png)



### chmod －更改文件模式

![image-20210503163828345](https://gitee.com/sxy22/note_images/raw/master/image-20210503163828345.png)

![image-20210503163852469](https://gitee.com/sxy22/note_images/raw/master/image-20210503163852469.png)

![image-20210503163859789](https://gitee.com/sxy22/note_images/raw/master/image-20210503163859789.png)



### su －以其他用户身份和组ID 运行一个shell

![image-20210706161700316](https://gitee.com/sxy22/note_images/raw/master/image-20210706161700316.png)



![image-20210706161817265](https://gitee.com/sxy22/note_images/raw/master/image-20210706161817265.png)



### sudo －以另一个用户身份执行命令

![image-20210706162058762](https://gitee.com/sxy22/note_images/raw/master/image-20210706162058762.png)



### chown －更改文件所有者和用户组

![image-20210503164425487](https://gitee.com/sxy22/note_images/raw/master/image-20210503164425487.png)

## 11 进程

## 12shell 环境

![image-20210504170154197](https://gitee.com/sxy22/note_images/raw/master/image-20210504170154197.png)

### 一些有趣的环境变量

![image-20210504170354246](https://gitee.com/sxy22/note_images/raw/master/image-20210504170354246.png)

![image-20210504170407389](https://gitee.com/sxy22/note_images/raw/master/image-20210504170407389.png)

### PATH

![image-20210504170758954](https://gitee.com/sxy22/note_images/raw/master/image-20210504170758954.png)



---









## 快捷键

### 移动光标

![image-20200825175752684](https://gitee.com/sxy22/note_images/raw/master/image-20200825175752684.png)

![image-20200825175805950](https://gitee.com/sxy22/note_images/raw/master/image-20200825175805950.png)



### 剪切

![image-20200825175918405](https://gitee.com/sxy22/note_images/raw/master/image-20200825175918405.png)



### 历史命令

![image-20200825180127149](https://gitee.com/sxy22/note_images/raw/master/image-20200825180127149.png)

## 文件目录类

### pwd

pwd  显示当前工作目录的绝对路径

### ls

ls [ 选 项] [目录或是文件]

• 常用选项

-a ：显示当前目录所有的文件和目录，包括隐藏的。

-l  ：以列表的方式显示信息

![image-20200820204540915](https://gitee.com/sxy22/note_images/raw/master/image-20200820204540915.png)

### cd

cd  [参数]     切换到指定目录

cd - 回到上一个工作目录

cd ~ 或者 cd ：回到自己的家目录

.当前目录

..父目录



### mkdir

mkdir  [选项]  要创建的目录

-p ：创建多级目录

### rmdir

rmdir  [选项]  要删除的空目录

rmdir 删除的是空目录，如果目录下有内容时无法删除的。

提示：如果需要删除非空目录，需要使用  rm -rf  要删除的目录



### touch 空文件

创建空文件



### cp/ 通配符

cp 指令拷贝文件到指定目录

• 基本语法

cp [选项] source dest

• 常用选项

-r ：递归复制整个文件夹

\cp 强制覆盖

![image-20200821205740237](https://gitee.com/sxy22/note_images/raw/master/image-20200821205740237.png)

![image-20200821210232736](https://gitee.com/sxy22/note_images/raw/master/image-20200821210232736.png)

![image-20200821210252189](https://gitee.com/sxy22/note_images/raw/master/image-20200821210252189.png)

![image-20200821210638553](https://gitee.com/sxy22/note_images/raw/master/image-20200821210638553.png)

### rm

rm 指令移除【删除】文件或目录

![image-20200821210935494](https://gitee.com/sxy22/note_images/raw/master/image-20200821210935494.png)

•  基本语法

rm  [选项]  要删除的文件或目录

•  常用选项

-r ：递归删除整个文件夹

-f ： 强制删除不提示



### mv 移动文件

•  基本语法

mv  oldNameFile newNameFile        (功能描述：重命名)

 mv  /temp/movefile  /targetFolder (功能描述：移动文件)

![image-20200821210859396](https://gitee.com/sxy22/note_images/raw/master/image-20200821210859396.png)



### cat 浏览文件

cat  [选项] 要查看的文件

•  常用选项

-n ：显示行号



cat 文件名 | more [分页浏览]



### more

more 指令是一个基于 VI 编辑器的文本过滤器，它以全屏幕的方式按页显示文本文件的内容

![image-20200810171640646](https://gitee.com/sxy22/note_images/raw/master/image-20200810171640646.png)

### less

less 指令用来分屏查看文件内容，它的功能与 more 指令类似，但是比 more 指令更加强大，支持各种显示终端。less 指令在显示文件内容时，并不是一次将整个文件加载之后才显示，而是根据显示需要加载内容，对于显示大型文件具有较高的效率。



![image-20200810172705871](https://gitee.com/sxy22/note_images/raw/master/image-20200810172705871.png)

###   > 指令 和 >> 指令

\> 输出重定向 : 会将原来的文件的内容覆盖

\>> 追加： 不会覆盖原来文件的内容，而是追加到文件的尾部

 ls -l >文件（功能描述：列表的内容写入文件 a.txt 中（覆盖写）

cat 文件 1 > 文件 2



### echo

echo 输出内容到控制台

### head

head 用于显示文件的开头部分内容，默认情况下 head 指令显示文件的前 10 行内容



•  基本语法

head  文件 (功能描述：查看文件头 10 行内容)

head -n 5 文件     (功能描述：查看文件头 5 行内容，5 可以是任意行数)



### tail

tail 用于输出文件中尾部的内容，默认情况下 tail 指令显示文件的后 10 行内容

tail -f  实时追踪文档的更新



### in

软链接也叫符号链接，类似于 windows 里的快捷方式，主要存放了链接其他文件的路径

ln -s [原文件或目录] [软链接名] （功能描述：给原文件创建一个软链接）

当我们使用 pwd 指令查看目录时，仍然看到的是软链接所在目录

![image-20200821211544491](https://gitee.com/sxy22/note_images/raw/master/image-20200821211544491.png)

![image-20200821211629625](https://gitee.com/sxy22/note_images/raw/master/image-20200821211629625.png)

### history

查看已经执行过历史命令,也可以执行历史指令

 

执行编号  !number

 



## 命令

![image-20201122161752858](https://gitee.com/sxy22/note_images/raw/master/image-20201122161752858.png)



### type

![image-20201122161957262](https://gitee.com/sxy22/note_images/raw/master/image-20201122161957262.png)

### which

![image-20201122162129396](https://gitee.com/sxy22/note_images/raw/master/image-20201122162129396.png)

![image-20201122162147705](https://gitee.com/sxy22/note_images/raw/master/image-20201122162147705.png)



### help

![image-20201122162336464](https://gitee.com/sxy22/note_images/raw/master/image-20201122162336464.png)



### --help

![image-20201122162424006](https://gitee.com/sxy22/note_images/raw/master/image-20201122162424006.png)



### man

![image-20201122162512676](https://gitee.com/sxy22/note_images/raw/master/image-20201122162512676.png)

![image-20201122162531059](https://gitee.com/sxy22/note_images/raw/master/image-20201122162531059.png)



### alias

![image-20201122162837199](https://gitee.com/sxy22/note_images/raw/master/image-20201122162837199.png)



## 时间类

### date

date "+%Y-%m-%d %H:%M:%S"（功能描述：显示年月日时分秒）

### cal

 

 ## 搜索查找

### find

find  [搜索范围]  [选项]

 ![image-20200811171110670](https://gitee.com/sxy22/note_images/raw/master/image-20200811171110670.png)

 

### locate

 locaate 指令可以快速定位文件路径。locate 指令利用事先建立的系统中所有文件名称及路径的locate 数据库实现快速定位给定的文件。Locate 指令无需遍历整个文件系统，查询速度较快。为了保证查询结果的准确度，管理员必须定期更新 locate 时刻。



由于 locate 指令基于数据库进行查询，所以第一次运行前，必须使用 updatedb 指令创建 locate 数据库



### grep  |

grep 过滤查找 ， 管道符，“|”，表示将前一个命令的处理结果输出传递给后面的命令处理。



grep [选项] 查找内容 源文件

![image-20200811172458612](https://gitee.com/sxy22/note_images/raw/master/image-20200811172458612.png)

![image-20200822211523261](https://gitee.com/sxy22/note_images/raw/master/image-20200822211523261.png)

## 压缩/解压

### gzip/gunzip



gzip 用于压缩文件，原来的文件不保留了， gunzip 用于解压的

gzip 文件   （功能描述：压缩文件，只能将文件压缩为*.gz 文件）

gunzip 文 件.gz （功能描述：解压缩文件命令）

![image-20200829210225724](https://gitee.com/sxy22/note_images/raw/master/image-20200829210225724.png)





### zip/unzip

zip 用于压缩文件， unzip 用于解压的，这个在项目打包发布中很有用的



•  基本语法

zip      [选项] XXX.zip  将要压缩的内容（功能描述：压缩文件和目录的命令）

unzip    [选项] XXX.zip （功能描述：解压缩文件）

•  zip 常用选项

-r：递归压缩，即压缩目录



•  unzip 的常用选项

-d<目录> ：指定解压后文件的存放目录



### tar

tar 指令 是打包指令，最后打包后的文件是 .tar.gz 的文件。

• 基本语法

tar  [选项]  XXX.tar.gz  打包的内容   (功能描述：打包目录，压缩后的文件格式.tar.gz)

![image-20200811173259436](https://gitee.com/sxy22/note_images/raw/master/image-20200811173259436.png)

![image-20200811173910376](https://gitee.com/sxy22/note_images/raw/master/image-20200811173910376.png)

## 文件所在组

### chown

chown [user] file

### chgrp

chgrp group file

除文件的所有者和所在组的用户外，系统的其它用户都是文件的其它组

### usermod 改变用户

 usermod   –g    组名  用户名

## 权限

### 权限说明

ls  -l 中显示的内容如下：

**-rwxrw-r--** 1 root root 1213 Feb 2 09:39 abc

第 0 位确定文件类型(d, - , l , c , b)

-普通文件，d目录， l软连接，c字符设备



第 1-3 位确定所有者（该文件的所有者）拥有该文件的权限。---User

第 4-6 位确定所属组（同用户组的）拥有该文件的权限，---Group

第 7-9 位确定其他用户拥有该文件的权限 ---Other





权限分为 r： 读， w： 写， x： 执行



rwx 作用到文件

[ r ]代表可读(read): 可以读取,查看

[ w ]代表可写(write): 可以修改,但是不代表可以删除该文件,删除一个文件的前提条件是对该文件所在的目录有写权限，才能删除该文件.

[ x ]代表可执行(execute):可以被执行



10.2.2    rwx 作用到目录

1) [ r ]代表可读(read): 可以读取，ls 查看目录内容

2) [ w ]代表可写(write): 可以修改,目录内创建+删除+重命名目录

3) [ x ]代表可执行(execute):可以进入该目录

![image-20200826200523858](https://gitee.com/sxy22/note_images/raw/master/image-20200826200523858.png)

![image-20200826200536189](https://gitee.com/sxy22/note_images/raw/master/image-20200826200536189.png)

### chmod 修改权限

u:所有者  g:所有组  o:其他人  a:所有人(u、g、o 的总和)

1) chmod   u=rwx,g=rx,o=x   文件目录名

2) chmod   o+w    文件目录名

3) chmod   a-x    文件目录名



规则：r=4 w=2 x=1            rwx=4+2+1=7 

chmod u=rwx,g=rx,o=x        

 文件目录名相当于 

chmod    751  文件目录名



### chown/chgrp 改变 所有者所有组

chown  newowner  file  改变文件的所有者

chown newowner:newgroup  file  改变用户的所有者和所有组

-R   如果是目录 则使其下所有子文件或目录递归生效





## crond 任务调度

### crontab

crontab [选项]

-e 编辑crontab 定时任务

-l 查询任务

-r 删除当前用户所有的crontab 任务



1)  cron -e

2)  */ 1 * * * * ls -l /etc >> /tmp/to.txt

3)  当保存退出后就程序。

4)  在每一分钟都会自动的调用 ls -l /etc >> /tmp/to.txt

![image-20200812163556579](https://gitee.com/sxy22/note_images/raw/master/image-20200812163556579.png)

![image-20200812164004168](https://gitee.com/sxy22/note_images/raw/master/image-20200812164004168.png)

![image-20200812170817570](https://gitee.com/sxy22/note_images/raw/master/image-20200812170817570.png)

### shell 执行

1、 编写文件.sh

2、 给文件可执行权限

3、 crontab -e 执行.sh文件



## RPM YUM



### rpm

查询已安装的 rpm 列表 rpm  –qa|grep xx



rpm -qa :查询所安装的所有 rpm 软件包rpm -qa | more [分页显示]



卸载： rpm -e RPM 包的名称

 rpm -e --nodeps foo

带上 --nodeps 就是强制删除



安装： rpm -ivh  RPM 包全路径名称

i=install 安 装

v=verbose 提 示

h=hash  进度条



 ### yum

yum list | grep xx 软件列表

yum install firefox



## 重定向

![image-20200822205407070](https://gitee.com/sxy22/note_images/raw/master/image-20200822205407070.png)

标准输入：

标准输出：命令的结果

标准错误信息：状态和错误信息



### 文件描述符(0,1,2)

重定向错误/状态信息

![image-20200822210526521](https://gitee.com/sxy22/note_images/raw/master/image-20200822210526521.png)



重定向标准输出和错误到同一个文件

![image-20200822210621247](https://gitee.com/sxy22/note_images/raw/master/image-20200822210621247.png)



### 输入重定向 |



![image-20200822210948554](https://gitee.com/sxy22/note_images/raw/master/image-20200822210948554.png)

可用 | ： head tail grep uniq sort

### tee

![image-20200822212102183](https://gitee.com/sxy22/note_images/raw/master/image-20200822212102183.png)



# shell



## 格式要求、 运行

+ 脚本以#!/bin/bash 开头

+ 要运行，给一个x权限或者sh ./file.sh



## 变量

Linux Shell 中的变量分为，系统变量和用户自定义变量



### 定义

变量名=值

撤销： unset 变量名

静态变量 readonly 变量名=值， 不能unset



### 规则

1)  变量名称可以由字母、数字和下划线组成，但是不能以数字开头。

2)  等号两侧不能有空格

3)  变量名称一般习惯为大写



### 将命令的返回值赋给变量

1） A=`ls -la` 反引号，运行里面的命令，并把结果返回给变量 A

2） A=$(ls -la) 等价于反引号



### 环境变量

export 变量名=值  功能描述：将 shell 变量输出为环境变量

 source /etc/profile  功能描述：让修改后的配置信息立即生效



### 位置参数变量（传入参数）





\$* （功能描述：这个变量代表命令行中所有的参数，$*把所有的参数看成一个整体）



\$@（功能描述：这个变量也代表命令行中所有的参数，不过$@把每个参数区分对待）

\$#（功能描述：这个变量代表命令行中所有参数的个数）

![image-20200815214129588](https://gitee.com/sxy22/note_images/raw/master/image-20200815214129588.png)



#### 预定义变量

$$ （功能描述：当前进程的进程号（PID））

$!  （功能描述：后台运行的最后一个进程的进程号（PID））

 


$？ （功能描述：最后一次执行的命令的返回状态。如果这个变量的值为 0，证明上一个命令正确执行；如果这个变量的值为非 0（具体是哪个数，由命令自己来决定），则证明上一个命令



### 运算符

1) “$((运算式))”或“$[运算式]”

2) expr m + n   注意 expr 运算符间要有空格

3) expr m - n

4) expr   \\*,  /,  %    乘，除，取余

![image-20200815214613596](https://gitee.com/sxy22/note_images/raw/master/image-20200815214613596.png)



### if/case/for/while

[ condition ]（注意 condition 前后要有空格）

1）整数比较

= 字符串比较

-lt 小 于

-le 小于等于

-eq 等 于

-gt 大 于

-ge 大于等于

-ne 不等于

2) 按照文件权限进行判断

-r 有读的权限 [ -r 文件 ]

-w 有写的权限

-x 有执行的权限

3)按照文件类型进行判断

-f 文件存在并且是一个常规的文件

-e 文件存在

-d 文件存在并是一个目录

#### if

•  基本语法

if [ 条件判断式 ];then

程序

fi

或者

if [ 条件判断式 ]

then

程序

elif [条件判断式]

then

程序

fi



![image-20200815215745892](https://gitee.com/sxy22/note_images/raw/master/image-20200815215745892.png)

#### case

case $变量名 in

"值 1"）

如果变量的值等于值 1，则执行程序 1

;;

"值 2"）

如果变量的值等于值 2，则执行程序 2

;;

…省略其他分支…

*）

如果变量的值都不是以上的值，则执行此程序



;;

esac



 


案例 1 ：当命令行参数是 1 时，输出  "周一", 是 2 时，就输出"周二"， 其它情况输出       "other"

#!/bin/bash

case $1 in

"1")

echo '周一'

;;

"2")

echo '周二'

;;

*)

echo 'other'

;;

esac



#### for



#### while

while [ 条件判断式 ]

do

程序

done



### read

读取控制台输入



### 函数

#### 系统函数

##### basename

•  basename 基本语法

功能：返回完整路径最后 / 的部分，常用于获取文件名

basename [pathname] [suffix]

![image-20200816171511286](https://gitee.com/sxy22/note_images/raw/master/image-20200816171511286.png)

##### dirname

功能：返回完整路径最后 / 的前面的部分，常用于返回路径部分

dirname 文件绝对路径 （功能描述：从给定的包含绝对路径的文件名中去除文件名（非目录的部分），然后返回剩下的路径（目录的部分）



#### 自定义函数

•  基本语法

 function  funname ()

{



Action; [return int;]

}

 

 

调用直接写函数名：funname  [值]

![image-20200816171818471](https://gitee.com/sxy22/note_images/raw/master/image-20200816171818471.png)

### 案例

需求分析

1)每天凌晨 2:10 备份 数据库 atguiguDB 到 /data/backup/db

2)备份开始和备份结束能够给出相应的提示信息

3)备份后的文件要求以备份时间为文件名，并打包成 .tar.gz 的形式，比如：

2018-03-12_230201.tar.gz

在备份的同时，检查是否有 10 天前备份的数据库文件，如果有就将其删除



#！ /bin/bash

BACKUP=/data/backup/db  #路径

TIME=$(date "+%Y-%m-%d_%H%M%S")

![image-20200816174523766](https://gitee.com/sxy22/note_images/raw/master/image-20200816174523766.png)



