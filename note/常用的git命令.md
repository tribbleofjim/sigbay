## 常用的git命令

本地创建仓库：git init

注意本地仓库必须创建文件并提交才能创建初始分支matser，可以随便添加一个文件，然后

git add .

git commit -m "xxxx"

git push

本地仓库关联远程仓库：git remote add origin xxxxxx

本地仓库首次推送：git push -u origin master

远程仓库也有东西，报fatal: refusing to merge unrelated histories：git pull origin master --allow-unrelated-histories 

查看本地git分支：git branch

查看所有（本地+远程）git分支：git branch -a

**把代码写到了另一个分支上**：git cherry-pick