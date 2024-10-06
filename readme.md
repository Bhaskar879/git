Importent website for git revise
```
Chai Docs
```
GIT command
```
pwd
cd one
$ git config --global user.email "example@gmail.com"
$ git config --global user.name "full name"
$ git config --list
```
Create reposetery
```
$ git init

git add .
git status
git commit -m "first commit"
git status

$ git log
$ git log --oneline

git commit
```
Branching
```
$ git branch
* master
$ git branch bug-fix
$ git switch bug-fix
$ git switch -c dark-mode
$ git checkout orange-mode
$ git checkout master
$ git merge bug-fix

$ git branch -m dark-mode black-mode
$ git branch -d orange-mode
```


Diff
```
$ git diff
$ git diff --staged
$ git diff 68df62f..68561ba
```
Stash
```
$ git stash
$  git checkout bug-fix

$ git stash save "Stach is temporal memory & behave like a stack "
$ git stash list

$ git stash apply
$ git stash drop
//OR
$ git stash pop

$git stash clear
```


Tag
```
$ git tag chai
$ git tag -a mchai -m "Release 1.0"
$ git tag

$ git log --oneline
$ git tag gchai 64538ab
```

Git Rebase,   
do all ways in sub branch  (Benifit: No extra commit happen)
```              
$ git switch -c purplemode
$ git add purple.txt
$ git commit -m "add purple mode"

$ git checkout master
$ git add fixes.txt
$ git commit -m "fix for purple mode"

$ git checkout purplemode

$ git rebase master
```

Git Reflog
(check precise history of commit) , recover deleted commit , refresh
``` 
$ git reflog
q
$ git log --oneline
$ git reset --hard 1fca7c7
$ git log --oneline                          
```