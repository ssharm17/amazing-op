###HW0:<br/>

###A. First four levels of the Git Branching exercise:<br/>

###Commands:<br/>
### 1. Introduction to Git Commits
```
git commit -m "C2"
git commit -m "C3"
```
### 2. Branching in Git
```
git checkout -b bugFix
```
### 3. Merging in Git
```
git branch bugFix
git checkout bugFix
git commit -m "C2"
git checkout master
git commit -m "C3"
git merge bugFix
```
### 4. Rebase Introduction
```
git checkout -b bugFix
git commit -m "C2"
git checkout master
git commit -m "C3"
git checkout bugFix
git rebase master
```

###Git Bonus:<br/>
### 1. Detach yo' HEAD
```
git checkout C4
```
### 2. Relative Refs (^)
```
git checkout bugFix^
```
### 3. Relative Refs #2 (~)
```
git branch -f master C6
git branch -f bugFix C0
git checkout HEAD~1
```
### 4. Reversing Changes in Git
```
git reset HEAD~1
git checkout pushed
git revert pushed
```
###Screenshot:<br/>
![image](https://cloud.githubusercontent.com/assets/3713160/14212381/93731a72-f800-11e5-8153-44f177915c75.png)

###B. Hooks:<br/>

###Contents of postcommit<br/>
```
#!/bin/sh

open https://www.google.com
```
###Screencast<br/>
[![Screencast](http://img.youtube.com/vi/59QCqt8FxXU/default.jpg)](http://www.youtube.com/watch?v=59QCqt8FxXU)