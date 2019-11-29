## 使用教程
先安装Git
```
  sudo apt-get install git
```
设置用户信息
```
  git config --global user.email "fyylvphy@pku.edu.cn"
  git config --global user.name "fyylvphy"
```

### 远程端同步代码三步走
将我们需要提交的代码（当前整个文件夹）从工作区添加到暂存区：
  git add .
将暂存区里的改动给提交到本地的版本库：
  git commit -m 'message'
将本地版本库的分支推送到远程服务器上对应的分支:
  git push #目前还不是很懂，输入这个后按照terminal上的提示操作即可
这时terminal会提示输入远程端用户名和密码，之后便可同步

查看当前状态用 git status


[廖雪峰的教程](https://www.liaoxuefeng.com/wiki/896043488029600/896827951938304#0)写得很好

要在github上删除一个仓库，在这个仓库的界面上点setting，然后拉到最后可以找到删除。
