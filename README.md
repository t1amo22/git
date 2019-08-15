# 提交记录

```js
git log  //查看提交记录
git log —oneline // 简化的提交记录
```

# 标签

```js
git tag <tagName> //本地打一个标签，一个tag对应一个commitId
git tag // 查看本地所有标签
git tag -d <tagName> // 删除标签
```

# push

```js
git push origin <tagName> //将标签推送到远端
git push origin —-tags  //推送所有标签
```

# 添加文件到暂存区

```js
git add . //添加本目录所有修改到暂存区
git add <pathName> //添加单个文件
git add -A . //添加本目录已跟踪和未跟踪文件的修改
```

# commit

```js
git commit -a -m ‘'
git commit -n -m ‘' //强制提交
```

# push

```js
git push <远程主机名> <本地分支> :<远程分支>

```
```js
git push origin master  //将本地master推送到远端的master
git push origin //把当前分支推送到origin主机的远程分支
git push origin HEAD //将当前分支推送到远端的同名分支
git push //远程只有一个当前的分支(只有一个主机origin)
```

# 查看分支

```js
git branch -r //查看远程分支
git branch -a //查看本地和远程分支
git branch //查看本地分支
```

# 撤销

```js
git checkout . //删除所有本地修改
git reset HEAD . //撤销暂存区的修改放到工作区
git reset —-hard HEAD^ //撤销上一次的commit并删除之前的代码
git reset —-hard commitId 
git reset —-soft HEAD^ //撤销上一次commit但不删除代码
```

# 取消跟踪

```
//.gitignore 文件添加不需要上传的文件 (node_modules)
git rm -r --cached <文件/文件夹名称>//删除远程分支
```
