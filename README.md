# git cheatsheet
Personal cheatsheet of commands that I commonly use when accessing VCS via the command line.
*(Not comprehensive)*

# initialization

### create a repo
```shell
touch README.md
git init
git add .
git commit -m <commit-msg>
git remote add origin <repository-url>
git remote -v
git push -u origin master
```
# push an existing repo
 
´´´shell
git remote add origin <repository-url>
git push -u origin master
´´´

# tracking changes
```shell
git status 
**or**
git diff
```
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
### revert a commit
```shell
git revert <commit-name>
**or**
git reset --hard <commit-name>
```
### remove uncommitted file
```shell
git rm <file-name>

```
# rebasing
```shell
git fetch origin
git rebase origin/master
```
### rebasing conflicts
```shell
git rebase --abort
**or**
git rebase --continue
```

# merging

### merging master into local branch
```shell
git fetch origin
git merge origin/master
```
### merge branch into local master
```shell
git merge <branch-name>
```
### merge conflicts
```shell
git rm <file-name>
```

# undoing

### undoing all lcoal changes before last commit
```shell
git reset --hard HEAD
```
