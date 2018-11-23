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
  > user.email=kai.cao@lynxi.com>
  credential.helper=store
  core.repositoryformatversion=0
  core.filemode=true
  core.bare=false
  core.logallrefupdates=true
  remote.origin.url=https://github.com/caok168/golangDemos.git
  remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*
  branch.master.remote=origin
  branch.master.merge=refs/heads/master
