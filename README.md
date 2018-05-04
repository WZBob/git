# git 常用命令
- git init   初始化本地仓库
- git clone -b branchName URL   clone远程仓库某分支
- git remote [-v] 查看远程仓库（包含简写，如origin）
- git remote add respName respURL  添加远程仓库（可命名简写）
- git remote rename respName1 respName2  重命名仓库简写
- git remote rm respName2  移除远程仓库
------

工作区  暂存区（stage） 
- git add file 把文件修改添加到暂存区
- git add . 判断所有被修改或删除的文档，及新增的文档，并将其信息追加到索引中
- git commit 将暂存区的所有内容提交到当前分支
- git push origin master  将修改合并到origin代表仓库的master分支

- git checkout -- file   可以丢弃工作区的修改，会获取暂存区的状态

------
