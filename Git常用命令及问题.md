# git@github.com:tian-0oO-ming/PublicDoc.git
# 常用命令
## git init 初始化git生成git仓库
## git status 查看git状态
## git add <filename>添文件到暂存区
## git add .加入所有文件到暂存区
## git commite -m 'message'提交文件到本地仓库
## git push 提交到远程仓库
## git reset <filename>将尚没有commite之前加入到暂存区的文件重新拉回

## git push [远程名] :[分支名]。 删除远程分支$ git push origin :master

## git branch -d master删除本地分支

#  文件状态：
## 1.没有被add过的文件叫untracked
## 2.add之后文件处于staged状态等待commite
## 3.commit之后文件处于unmodified这里之所以是modified是因为文件会跟仓库中的文件对比
## 4.当unmodified的文件被修改则会变为modified状态
## 5.modified之后的文件add之后将继续变为staged状态
## 6.unmodifed的文件还有一种可能是已经不再需要了，那么可以remove它不再追踪变为untracked状态




# 远程的代码没有先clone到本地，所以不兼容。
```
解决办法是：
在git pull和git push命令中添加–allow-unrelated-histories
让git允许提交不关联的历史代码。
git pull origin master --allow-unrelated-histories   
```
