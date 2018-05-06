# git 常用命令
- git init   初始化本地仓库
- git clone -b branchName URL   clone远程仓库某分支
- git remote [-v] 查看远程仓库（包含简写，如origin）
- git remote add respName respURL  添加远程仓库（可命名简写）
- git remote rename respName1 respName2  重命名仓库简写
- git remote rm respName2  移除远程仓库
- git status  查看当前工作树的状态
------

工作区  暂存区（stage） 
- git add path 把文件修改添加到暂存区。对删除已被git管理的文件，没必要用add，直接commit就可以
- git add . 判断所有被修改或删除的文档，及新增的文档，并将其信息追加到暂存区
- git add -u [path] 将path中所有tracked文件中被修改或删除文件的信息添加到暂存区，不会处理untracked文件。
- git add -A [path] 将path中所有tracked文件中被修改或删除文件和所有untracked的文件信息添加到暂存区
- git commit -m "描述"  将暂存区的所有内容提交到当前分支
- git commit -a -m "描述"  只将被修改或删除的被git管理的文件提交到仓库（在不使用add命令时）
- git push origin master  将修改合并到origin代表仓库的master分支

- git checkout -- path   可以丢弃工作区的修改，会获取暂存区的状态

------
拉取远程更新到本地
- git pull 仓库简写  远程分支:本地分支

	git pull origin new:master  将origin中的new分支，与本地master分支合并
	git pull origin new         将origin中的new分支，与本地当前分支合并
	git pull origin             将origin中的当前分支与本地分治合并
	git pull                    拉去当前分支对应的远程分支
