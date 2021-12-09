# 1 版本控制系统
![本地版本控制系统](本地版本控制系统.png "本地版本控制系统")
![集中化版本控制系统](集中化版本控制系统.png "集中化版本控制系统")
![分布式版本控制系统](分布式版本控制系统.png "分布式版本控制系统")
![版本控制系统](版本控制系统.jpg "版本控制系统")

<br>
<br>

# 2 Git概念机制
## 2.1 三种状态 / 三种区域
![三种状态区域](三种状态区域.jpg "三种状态区域")
![三种状态](三种状态.png "三种状态")
![三种区域](三种区域.png "三种区域")

<br>
<br>

## 2.2数据记录机制
![数据记录机制](数据记录机制.jpg "数据记录机制")
![数据记录机制](数据记录机制.png "数据记录机制")

<br>
<br>

## 2.3 每次commit生成的对象
![每次commit生成的对象](每次commit生成的对象.jpg "每次commit生成的对象")
![多个commit对象](多个commit对象.png "多个commit对象")
![一个commit对象](一个commit对象.png "一个commit对象")

<br>
<br>

# 3 Git安装配置
## 3.1 Git安装
> Win&emsp;http://git-scm.com/download/win
<br>
> Mac&emsp;Terminal输入git回车即可

<br>
<br>

## 3.2 Git客户端
>最流行客户端清单&emsp;https://git-scm.com/downloads/guis
<br>
>更全面客户端清单&emsp;https://git.wiki.kernel.org/index.php/Interfaces,_frontends,_and_tools#Graphical_Interfaces

<br>

### 原生 - gitk 历史记录的图形化查看器(命令gitk)
![gitk](gitk.png "gitk")

<br>

### 原生 - git-gui制作提交的工具(命令git gui)
![git-gui](git-gui.png "git-gui")

<br>
<br>

## 3.3 Git配置
>### 优先级：项目 > 用户 > 系统

```
git config --list --show-origin      所有配置
git config --system                  系统配置文件  /etc/gitconfig
git config --global                  用户配置文件  ~/.gitconfig 或 ~/.config/git/config
git config --local(项目目录下默认)      项目配置文件  .git/config
```

<br>
<br>

# 4 Commit规范

## 4.1 常见commit习惯

>### git commit -m "推送详情页导航栏"
>### git commit -m "feat: 推送详情页导航栏"
>### git commit -m "feat(推送功能): 推送详情页导航栏"
<br>

## 4.2 commitizen规范
>### git commit -m "类别(影响范围): 简短描述"
<br>

```
类别
feat         新功能(feature)
fix          修补bug
docs         文档(documentation)
style        格式(不影响代码运行的变动)
refactor     重构(即不是新增功能，也不是修改bug的代码变动)
perf         性能优化
test         增加测试
chore        构建过程或辅助工具的变动
...
```

## 4.3 个人建议

>### git commit -m "feat(分支功能名): 推送详情页导航栏"
>### git commit -m "fix(bug单号): 推送详情页导航栏"

<br>
<br>

# 5 分支操作
![分支操作理解](分支操作理解.jpg "分支操作理解")

<br>

![分支操作](分支操作.png "分支操作")
```
master分支
常规开发新功能
git checkout -b c5
git commit -a -m 'feat(c5): c5功能'

临时任务
git checkout master
git checkout -b c4
git commit -a -m 'feat(c4): c4功能'

临时任务合并
git checkout master
git merge c4        ----快进合并

继续开发之前新功能
git checkout c5
git commit -a -m 'feat(c5): c5功能'

新功能合并
git checkout master
git merge c5        ----三方合并

三方合并冲突 (同一个文件两方都修改)
git status             查看冲突文件
解决方式                手动(推荐) / git mergetool
git merge --abort      合并失败中止
git commit -a -m ""    合并成功提交

```

# commit简写

# 重置操作

# 撤销操作

# 重写历史

# Git Submodule
