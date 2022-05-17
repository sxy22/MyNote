 

# Pro Git

## Git 基础

```
git config --global user.name "Sicheng He"
git config --global user.email "sichengh1997@gmail.com"
git remote add origin git@github.com:User/UserRepo.git
# 检查配置
git config --list
```





### git init

![image-20210321214504308](https://gitee.com/sxy22/note_images/raw/master/image-20210321214504308.png)



###  git clone

![image-20210321214548317](https://gitee.com/sxy22/note_images/raw/master/image-20210321214548317.png)



### git status  检查当前文件状态

![image-20220517100727017](https://gitee.com/sxy22/note_images/raw/master/img/image-20220517100727017.png)



###  git add 跟踪

![image-20210321214834175](https://gitee.com/sxy22/note_images/raw/master/image-20210321214834175.png)

### 忽略文件

![image-20210321215124754](https://gitee.com/sxy22/note_images/raw/master/image-20210321215124754.png)

![image-20210321215208738](https://gitee.com/sxy22/note_images/raw/master/image-20210321215208738.png)

### git commit 提交更新

### git rm 移除文件

![image-20210321215632348](https://gitee.com/sxy22/note_images/raw/master/image-20210321215632348.png)

![image-20210321215740959](https://gitee.com/sxy22/note_images/raw/master/image-20210321215740959.png)



### git mv 移动文件

![image-20220517101654618](https://gitee.com/sxy22/note_images/raw/master/img/image-20220517101654618.png)





### git log 查看日志



### 撤销commit操作

![image-20220517102133502](https://gitee.com/sxy22/note_images/raw/master/img/image-20220517102133502.png)

### git reset取消暂存的文件

![image-20220517102959080](https://gitee.com/sxy22/note_images/raw/master/img/image-20220517102959080.png)



### 撤销文件的修改

![image-20220517103052790](https://gitee.com/sxy22/note_images/raw/master/img/image-20220517103052790.png)

### git remote 查看github

![image-20220517103444683](https://gitee.com/sxy22/note_images/raw/master/img/image-20220517103444683.png)



### 添加远程仓库

![image-20220517103941428](https://gitee.com/sxy22/note_images/raw/master/img/image-20220517103941428.png)





## Git 分支



### 分支创建

![image-20210324231111040](https://gitee.com/sxy22/note_images/raw/master/image-20210324231111040.png)



### 分支切换

![image-20210324231135008](https://gitee.com/sxy22/note_images/raw/master/image-20210324231135008.png)

### 分支的新建与合并

![image-20210324231539322](https://gitee.com/sxy22/note_images/raw/master/image-20210324231539322.png)























# git



![image-20210218202650959](https://gitee.com/sxy22/note_images/raw/master/image-20210218202650959.png)

![image-20210218203023195](https://gitee.com/sxy22/note_images/raw/master/image-20210218203023195.png)

### 本地库

git init 初始化

git config user.name HeSicheng

git config user.email sh53@Illinois.edu



git status  查看本地库状态

git add file 加入暂存区

git rm --cached file 从暂存区移除



git commit -m ”message“ file 不用打开vim就可以写message



git log 查看日志

git reflog 

### 切换版本

 git reset --hard 版本号

![image-20210218214112208](https://gitee.com/sxy22/note_images/raw/master/image-20210218214112208.png)

### 比较文件差异

git diff 与暂存区比较

git diff 版本号 与历史比较

![image-20210218215227034](https://gitee.com/sxy22/note_images/raw/master/image-20210218215227034.png)

### 分支

git branch -v 查看分支

git branch 分支名 创建分支

git checkout 切换分支

git merge 合并分支

![image-20210219001157338](https://gitee.com/sxy22/note_images/raw/master/image-20210219001157338.png)

# github

### push & clone

git remote add [别名] [repo地址]

git push [地址别名] [分支名]

git clone 地址

![image-20210219150512155](https://gitee.com/sxy22/note_images/raw/master/image-20210219150512155.png)

### fetch & pull

![image-20210219151445196](https://gitee.com/sxy22/note_images/raw/master/image-20210219151445196.png)

### 冲突

![image-20210219152110499](https://gitee.com/sxy22/note_images/raw/master/image-20210219152110499.png)

### fork & pull request

先fork

本地修改

push

pull request





https://htmlpreview.github.io/?https://github.com/sxy22/test/blob/master/lec5-2.html





```
git config user.name "SICHENG HE"
git config user.email "sichengh1997@gmail.com"
git remote add origin git@github.com:User/UserRepo.git
```







