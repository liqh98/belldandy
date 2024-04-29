## using the git command

using tools in the goal

## init 
git init .
git config --global user.name "name"
git config --global user.email "email"
git config --global list


## commit & push

git add . ;; add all file to the repository.(index? cache?)
git commit -m "message"
git push
git clone git@github.com:name/repository/name

## branch
git branch new_name
git checkout change_name
git checkout -b name;;  git branch name, git checkout name
git merge name
git branch -d name;; to delete the branch

git branch
git branch -v
git branch --merged
git log --oneline --decorate --graph --all

## others

git status ;; to see all the state
