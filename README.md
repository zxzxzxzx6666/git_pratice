# LEARN GIT
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
    // remote add <remote(shortname fot git web site)> <git web>
    git remote add origin git@github.com:zxzxzxzx6666/git_pratice.git
    // git push -u <remote> <branch>
    git push -u origin main

# 二、git basic
## 01 check
    // list config information
    git config --list
    // to know now branch
    git status
    // show logs
    git log
    git log --oneline --decorate
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
    // after add to stage we can use reset to reset that !! will delete !!
    git reset --HEAD .\README.md
    // !! will create new push !!
    git revert --HEAD --no-edit
## 04 remote 
    // check now remote Repositories
    $ git remote
    // show all remote
    $ git remote -v
    // change remote
    git remote set-url <remote_name> <remote_url>
    // change remote git fetch <origin>
    git fetch test
    // remove remote
    git remote remove test
## 05 tag
    // list tag
    git tag
    // add tag for now
    git tag -a v1.4 -m "my version 1.4"
    git push
## 06 Aliases
    // set aliases
    git config --global alias.last 'log -1 HEAD'
    // use it 
    $ git last
    (you can see the last commit easily)
# 三、branch
## 01 basic
    // show branches and if up to date
    git remote show origin
    // show branch (no merged)
    git branch --no-merged
    // create branch
    git branch testing
    // switch branch
    git checkout testing
    // merge bridge
    git merge hotfix
    // delete bridge
    git branch -d hotfix
## 02 head
    // check head on which branch
    cat .git/HEAD
    // point to version (need to change to the branch first)
    git checkout <指定 commit SHA-1>