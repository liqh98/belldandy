## using the git command

using tools in the goal; perhap git graph tool to use in vscode


## init 
```
git init .
git config --global user.name "name"
git config --global user.email "email"
git config --global list
```

## commit & push
```
git add . ;; add all file to the repository.(index? cache?)
git commit -m "message"
git push
git clone git@github.com:name/repository/name
git pull
```
## branch
```
git branch new_name
git checkout change_name
git checkout -b name;;  git branch name, git checkout name
git merge name
git branch -d name;; to delete the branch

git branch
git branch -v
git branch --merged
git log --oneline --decorate --graph --all
```
## remote

git remote add origin https://github.co/OWNER/repository.git
git remote -v
git remote set-url
    * https://github.com/owner/repository.git
    * git@github.com:owner/repository.git
git remote set-url origin git@github.com:liqh98/linux-c.git
git remote rename oldname newname
> git remote rename origin destination
git remote rm destination(name)
git push --set-upstream origin main

如果远程仓库和现有仓库发生冲突。
1. 对新的远程仓库使用不同名称
2. 重命名现有的远程仓库
3. 添加新仓库前删除现有远程仓库

## others
```
git status ;; to see all the state
```
感觉我就已经遭遇了一次变基？
我在本地环境进行修改，然后add 加入了分支里，之后想要提交 git push
在这之前我在另一个地方，对服务器上的远程文件进行了修改，然后保存了提交。
所以发生了不让我提交的冲突，
git fetch 可以，但是git pull 失败了，git pull rebase 成功了，到底是怎么回事？


### create a new repository
git init
git init -b main
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/liqh/linux-c.git
git push -u origin main
git remote -v

## github commandline tools
cli.github.com/manual/
gh auth login
用来进行验证登陆
gh config list; gh config set editor vim
### gh repo

gh repo view owner/repo
gh repo clone owner/repo
gh repo create
gh pr list --repo owner/repo
gh repo list
gh repo create ;; 交互式的创建过程
gh repo create --source=. --public --remote=upstream
gh repo set-dafault 
gh repo edit ;; edit repository settings
### gh other tools

gh ; gh to know top github cli command list
gh status


#### 将本地代码提交到远程仓库
* 使用github cli
* 使用 github desktop
* 将现有源码添加
