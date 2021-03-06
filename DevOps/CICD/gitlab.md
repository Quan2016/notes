# 博客
[git bash环境设置](https://blog.csdn.net/jingtingfengguo/article/details/51892864)
[git相关原理和常用命令](https://segmentfault.com/a/1190000017114656)

# 命令
```
git config -l #查看config配置
git status #查看文件状态
git branch [name] #创建分支
git checkout [name] #切换分支或者检出文件
git pull #拉取代码
git pull orgin master
git push #推送代码 使用方法:git push <远程主机名> <本地分支名>:<远程分支名>
# 上传本地指定分支到远程仓库
git push origin [name]
git checkout#命令用于切换分支或恢复工作树文件
tag创建
git tag v1.0#创建标签
git  tag v0.9 471fd27#对指定commit打tag
git push origin v0.9#push单个tag
git push --tags#push所有tag
git reset --hard#从历史中恢复
git push origin source -f
git reset --mixed文件退出暂存区 git add . 发现多add了文件，要重新add的时候
git push origin --delete <BranchName>#删除远程分支
git branch -d <BranchName>#删除本地分支

git stash drop
git stash pop stash@{0}
git stash list


## 恢复
#删除暂存区和分支的文件
git rm --cached file_path
#将file回退到unstage区
git reset HEAD
#修改最后一次提交
 git commit --amend
```
fork的代码同步

```
#添加项目A的远程仓库地址到upstream
git remote add upstream <你朋友项目A的仓库地址>

#把项目A的更新来到本地的upstream里
git fetch upstream

#切换到你自己想要merge的分支，这里我用举例：master
git checkout master

#merge项目A的更新到你的branch
git merge upstream/master
```



# 书籍

[pro git](https://gitee.com/progit/)

[pro git2](https://progit.bootcss.com/)
---
#其他有用的命令
```
git config --global credential.helper cache #缓存账号密码
git config --global http.sslVerify false  #报SSl错误

```



> HEAD严格来说不是指向提交，而是指向master，master才是指向提交的，所以，HEAD指向的就是当前分支

