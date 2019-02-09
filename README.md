# github cheatsheet
Cheatsheet of git commands

# branches

### checking all branches
```shell
git branch --all
```
### creating a branch
```shell
git checkout -b <branch-name>
```

### deleting a remote branch
```shell
git push --delete origin <branch-name>
```
### deleting a local branch
```shell
git branch -D <branch-name>
```
# rebasing
```shell
git fetch origin
git rebase origin/master
```
# merging

### merging master into local branch
```shell
git fetch origin
git merge origin/master
```
