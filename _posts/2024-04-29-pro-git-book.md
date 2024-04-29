## using the git command

using tools in the goal; perhap git graph tool to use in vscode


## init 
```git init .
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
## others
```
git status ;; to see all the state
```
感觉我就已经遭遇了一次变基？
我在本地环境进行修改，然后add 加入了分支里，之后想要提交 git push
在这之前我在另一个地方，对服务器上的远程文件进行了修改，然后保存了提交。
所以发生了不让我提交的冲突，
git fetch 可以，但是git pull 失败了，git pull rebase 成功了，到底是怎么回事？
