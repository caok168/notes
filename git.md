## git 命令

* git add . //把当前文件添加到暂存区
* git reset -- files //撤销暂存区文件   用来撤销最后一次git add files，你也可以用git reset    撤销所有暂存区域文件
* git commit -m ""  //给暂存区域生成快照并提交

* git checkout [file] //恢复暂存区的指定文件到工作区
* git checkout .   //恢复暂存区的所有文件到工作区
* git checkout [commit] [file]  //恢复某个commit的指定文件到暂存区和工作区

* git reset --hard  //重置暂存区与工作区，与上一次commit保持一致
* git reset --hard [commit]  //重置当前分支的HEAD为指定commit，同时重置暂存区和工作区，与指定commit一致

* git config 
* git config -l  //列出所有

  > user.name=Kai Cao </br>
  > user.email=kai.cao@lynxi.com> </br>
  credential.helper=store </br>
  core.repositoryformatversion=0 </br>
  core.filemode=true </br>
  core.bare=false </br>
  core.logallrefupdates=true </br>
  remote.origin.url=https://github.com/caok168/golangDemos.git </br>
  remote.origin.fetch=+refs/heads/*:refs/remotes/origin/* </br>
  branch.master.remote=origin </br>
  branch.master.merge=refs/heads/master </br>

* git stash
* git stash list //查看所有的stash
* git stash drop //移除stash,后面可以跟着stash名字  git stash drop stash@{0}
* git stash clear //移除所有的stash
* git stash show //查看指定stash的diff ,后面可以跟着stash名字,在该命令后面添加-p或--patch可以查看特定stash的全部diff
* git stash pop  //可以通过git stash pop命令恢复之前缓存的工作目录
* git stash apply  //将缓存堆栈中的stash多次应用到工作目录中，但并不删除stash拷贝
