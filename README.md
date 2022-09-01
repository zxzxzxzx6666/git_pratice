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
## 01 config 
    // list config information
    git config --list
## 02 Recording Changes to the Repository
    // to know now branch
    git status
    // add new file untracked
    git add CONTRIBUTING.md
    // check difference
    git diff
    // compares your staged changes to your last commit
    git diff --staged
    // git commit 
    git commit -m "Story 182: fix benchmarks for speed"
 
