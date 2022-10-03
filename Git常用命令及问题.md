# git@github.com:tian-0oO-ming/PublicDoc.git

# 常用命令

## git init 初始化 git 生成 git 仓库

## git status 查看 git 状态

## git add <filename>添文件到暂存区

## git add .加入所有文件到暂存区

## git commite -m 'message'提交文件到本地仓库

## git push 提交到远程仓库

## git reset <filename>将尚没有 commite 之前加入到暂存区的文件重新拉回

## git push [远程名] :[分支名]。 删除远程分支$ git push origin :master

## git branch -d master 删除本地分支

# 修改已创建项目的主分支为 main

## 切换到主分支 master

## 使用 git branch -M main 命令, 把当前 master 分支改名为 main, 其中-M 的意思是移动或者重命名当前分支

# 文件状态：

## 1.没有被 add 过的文件叫 untracked

## 2.add 之后文件处于 staged 状态等待 commite

## 3.commit 之后文件处于 unmodified 这里之所以是 modified 是因为文件会跟仓库中的文件对比

## 4.当 unmodified 的文件被修改则会变为 modified 状态

## 5.modified 之后的文件 add 之后将继续变为 staged 状态

## 6.unmodifed 的文件还有一种可能是已经不再需要了，那么可以 remove 它不再追踪变为 untracked 状态

# 远程的代码没有先 clone 到本地，所以不兼容。

```
解决办法是：
在git pull和git push命令中添加–allow-unrelated-histories
让git允许提交不关联的历史代码。
git pull origin master --allow-unrelated-histories
```
