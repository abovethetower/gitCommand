# git命令的使用

## 一、使用git将文件通过ssh传输到github上
- 首先要初始化Git[^1]
- 然后使用git add filename将文件添加到暂存区
- 再使用git commit -m "详细的提交描述信息"提交文件到本地仓库
- 先在Github上创建一个空的远程仓库（不初始化README文件）关联远程Github仓库（git remote add origin 远程仓库的地址）
```
git remote add origin https://github.com/abovethetower/yourrepository.git
```
- 最后使用git push 命令将本地提交推送到Github。
```
git push -u origin main
``` 
参数u表示设定上游分支，在首次推送时使用，后续推送直接使用git push即可。

[^1]:在该目录下用git init来创建一个新的Git仓库。

##二、如何从远程仓库克隆
使用git clone命令
```
SSH
git clone git@github.com:username/reponame.git
```
```
HTTPS
git clone https://github.com/username/reponame.git
```
