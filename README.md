# hello-world
This is my fist hello-world!
I am very exciting to do this!
I am looking forward to the interesting thing!
Ok！
- git init   初始化本地仓库
- git clone -b branchName URL   clone远程仓库某分支
- git remote [-v] 查看远程仓库（包含简写，如origin）
- git remote add respName respURL  添加远程仓库（可命名简写）
- git remote rename respName1 respName2  重命名仓库简写
- git remote rm respName2  移除远程仓库

工作区  暂存区（stage） 
- git add 把文件修改添加到暂存区，对于只修改或删除已被git管理的文档，没必要使用add，可以使用commit
- git add . 判断所有被修改或删除的文档，及新增的文档，并将其信息追加到索引中
- git commit 将暂存区的所有内容提交到当前分支
