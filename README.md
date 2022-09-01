# 一、Getting Started 
## 01 Getting a Git Repository
    // first create a Repository on git website
    // deploy keys in Setting on git website for no password push
    toutch README.md
    git init
    git add README.md
    touch README.md
    git add README.md
    git commit -m "first commit"
    git remote add origin git@github.com:zxzxzxzx6666/git_pratice.git
    git push -u origin main

# 二、git basic
## 01 check
    // list config information
    git config --list
    // to know now branch
    git status
    // show logs
    git log
## 02 simple commit
    // to know now branch
    git status
    // check difference
    git diff
    // compares your staged changes to your last commit
    git diff --staged
    // add new file untracked or modified
    git add CONTRIBUTING.md
    // git commit 
    git commit -m "add some words"
    // push
    git push
## 03 undo things
    // after add to stage we can use reset to reset that
    git reset --HEAD .\README.md
