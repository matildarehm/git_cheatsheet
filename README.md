# git cheatsheet
> Personal cheatsheet of commands that I commonly use when accessing VCS via the command line.
*(Not comprehensive)*

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
# commits

### show all commits
```shell
git log
```
### see who altered file
```shell
git blame <file-name>
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
