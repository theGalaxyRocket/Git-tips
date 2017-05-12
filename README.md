![](http://oo8jzybo8.bkt.clouddn.com/hello-github.jpg)

## GitHub介绍
GitHub 是为开发者提供 Git 仓库的托管服务。这是一个让开发者与朋友、同事、同学及陌生人共享代码的完美场所。总结一下，GitHub 最大的特征是“面向人”

Git是一个“**分布式版本管理工具**”，简单的理解版本管理工具：大家在写东西的时候都用过“回撤”这个功能，但是回撤只能回撤几步，假如想要找回我三天之前的修改，光用“回撤”是找不回来的。而“**版本管理工具**”能记录每次的修改，只要提交到版本仓库，你就可以找到之前任何时刻的状态（文本状态）。

* **统一概念**

    * 工作区：改动（增删文件和内容）
    * 暂存区：输入命令：`git add 改动的文件名`，此次改动就放到了‘暂存区’
    * 本地仓库(简称：本地)：输入命令：`git commit 此次修改的描述`，此次改动就放到了’本地仓库’，每个commit，我叫它为一个‘版本’。
    * 远程仓库(简称：远程)：输入命令：`git push 远程仓库`，此次改动就放到了‘远程仓库’（GitHub等)
    * commit-id：输出命令：`git log`，最上面那行`commit xxxxxx`，后面的字符串就是commit-id

Blog:[【GitHub Desktop】MacOS和Win下配置及简单的使用](http://www.cnblogs.com/SeekHit/p/6257451.html)

## Tips
### 添加暂存区
```sh
#把工作时的所有变化提交到暂存区，包括文件内容修改(modified)以及新文件(new)，但不包括被删除的文件。
git add .   

#仅监控已经被add的文件,不会提交新文件（untracked file）
git add -u

#是上面两个功能的合集（git add --all的缩写）
git add -A
```
### 本地仓库
```sh
git commit -m "描述"
```

### 提交远程仓库
```sh
git push
```
### 从远程仓库拉取
```sh
git pull
```
