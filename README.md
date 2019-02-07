# github cheatsheet
Cheatsheet of git commands

# branches

### checking all branches
```shell
git branch --all
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
