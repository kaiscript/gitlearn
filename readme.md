1.基本命令

- git add 将工作区内容提交到暂存区
- git commit -f <file> -m <msg> 提交文件
- git status
- git log 本次工作历史
- git reset --hard <version> 回滚
- git reflog 仓库操作历史
- git checkout -- <file> 丢弃工作区的更改
- git rm <file> 删除文件

2.远程

- git remote add origin git@server-name:path/repo-name.git  关联一个远程库
- git push -u origin master 第一次推送master分支的所有内容
- git push origin master 
  本地提交后，推送最新修改

3.分支管理

- git checkout -b dev   
  创建并切换分支
  相当于以下2个命令
- $ git branch dev
- $ git checkout dev

---

- git branch 查看当前分支
- git branch <name> 创建分支
- git checkout <name> 切换分支
- git checkout -b <name>  创建+切换分支
- git merge <name>  合并到dev分支
- git branch -d <name> 删除分支
- git merge --no-ff -m "merge with no-ff" dev  
  禁用Fast forward模式，删除分支后不会丢失分支信息

---

- git stash 存储现场
- git stash list 
- git stash apply <name> 恢复现场
- git stash drop 删除现场

---

- git branch -D <name> 强行删除分支
