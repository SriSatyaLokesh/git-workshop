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