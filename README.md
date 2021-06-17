### Git Basics and useful commands

#### git config
- configure author name and email adress
- git config –global user.name `“name”`

- git config –global user.email `“email address”`
```
git config –global user.name "MyName"

git config –global user.email "myname@mymail.com"
```
#### git init
- Initialize git in your repository
- git init `repository name`
```
git init [OR] git init \home\desktop\repoName
```
#### git clone
- to clone a remote repository
- git clone `url`
```
git clone https://github.com/SriSatyaLokesh/git-workshop
```
#### git add
- to add files to staging (commit list)
- git add `filename`
- git add . - to add all files
```
git add README.md
git add .
```
#### git diff
- to see what files are in staging, what are changes made
- git diff
    - changes which aren't staged
- git diff -staged
    - changes that are staged
- git `branch 1` `branch 2`
    - check differences between branches
#### git commit
- to commit changes made in file, each commit is a save point.
- git commit -m `"commit message"`
```
git commit -m "Added README.md"
```
#### git reset
- to unstage a file
- git reset `file`
- git reset `commit ID`
    - undo commit changes [preserves a copy]
- git reset --hard `commit ID`
    - undo commit changes and discards
#### git status
- shows files that are to be commited
```
git status
```
#### git rm
- to remove a file from git repo
```
git rm README.md
```
#### git log 
- to see commit log, everything abour commits - what, when, who, where
``` 
git log
``` 
#### git show 
- to see what all changes are done in a commit
- git show `commit ID`

Let's start working woth branches 
![branches](https://www.nobledesktop.com/image/gitresources/git-branches-merge.png)
#### git branch
- `git branch`
    - lists all branch names
- `git branch "branch name"`
    - creates a new branch
- `git branch [-d] [-D] "branch name"`
    - [-d] - Soft Delete
    - [-D] - Hard Delete
#### git checkout 
- to swich between branches
- `git checkout "branch name"`
    - to switch to specified branch
- `git checkout -b "branch name"`
    - create and switch a branch from current branch
#### git merge
- `git merge "branch name"`
    - merges given branch in the current branch

Let's colloborarw with others usinf remote repos
![Remote repos](https://www.cs.swarthmore.edu/~newhall/unixhelp/gitrepos.gif)
#### git remote
- to connect your local repo to the remote repo
- git remote add origin `"Remote Server Link"` 
```
git add origin https://github.com/SriSatyaLokesh/git-workshop
```
#### git push
- to push your commits from local repo to remote repo
- git push origin `"branch name"`
    - to push specified branch changes
- git push -all
    - push all branches
#### git pull
- to pull remote changes into local repo
- git pull `"remote repo URL"`
```
git pull https://github.com/SriSatyaLokesh/git-workshop
````
#### git stash and pop
- just to save the copy of changes, before switching branches and can revert back using pop
![stash and pop](https://static.javatpoint.com/tutorial/git/images/git-stash.png)

#### other commands
- cherry-pick
- rebase
- etc