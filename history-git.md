# Git History
This is my history of learning about git.


## Purpose
- Learning Github
- Learning Git commands
- Learning English


## What I learned

2017/01/09

1. How to send pull-request from cloned repository
 - Clone repository and create a branch for updating.
    ```bash
    $ mkdir update-pullreq
    $ cd update-pullreq
    $ git clone https://github.com/mike-r155/edu-git.git
    ```

 - Checkout it and update.
    ```bash
    $ git checkout -b update-pullreq
    ... update ...
    $ git add -A
    $ git commit -m "[update] add pullreq"
    ```

 - Push the branch to GitHub.
    ```bash
    $ git push origin update-pullreq
    ```

 - Access to GitHub and click "Compare & pull request" button.
 - Write some comment and click "Send pull request" button.

2. How to merge from pull-request

	
2017/01/06

1. How to use local ssh server
 - New git commands:
    - Create empty repository for server
    ```bash
    $ mkdir project.git
    $ cd project.git
    $ git --bare init
    ```

    - Show origin URL
    ```bash
    $ git remote -v
    ```

    - Change remote repository URL
    ```bash
    $ git remote set-url origin xxx@192.168.1.3:/home/xxx/project.git
    $ git push -u origin mater
    ```

2017/01/04

1. Resolve conflict
 - New git commands:
    - Create branch and checkout it
    ```bash
    $ git checkout -b conf-branch
    ```

    - Amend last comment
    ```bash
    $ git commit --amend
    ```

    - Remove existing file from HEAD
    ```bash
    $ git rm ./conflict.txt
    ```

2. Manage HEAD
 - New git commands:
    - Change HEAD to previous
    ```bash
    $ git reset --soft HEAD~
    ```

    - Undo previous reset
    ```bash
    $ git reset --soft ORIG_HEAD
    ```

    - Show HEAD changing log and reset from it
    ```bash
    $ git reflog
    $ git reset --soft HEAD@{5}
    ```

 - Note:
    - HEAD is current commit
    - HEAD~(or HEAD^) is previous commit of HEAD
    - ORIG_HEAD is previous HEAD before reset
    - Use reflog if you want to reset to future HEAD point

3. Fork of GitHub AndroidTraining repository
 - New git commands:
    - Clone from GitHub
    ```bash
    $ git clone https://github.com/mike-r155/AndroidTraining.git
    ```

2017/01/04

1. Create branch and merge it.
 - New git commands:
    - Create branch
    ```bash
    $ git branch
    $ git testbranch
    $ git checkout testbranch
    ```

    - Check commit log with branch status
    ```bash
    $ git log --oneline --decorate
    ```

    - Merge to master and delete the branch
    ```bash
    $ git checkout master
    $ git merge testbranch
    $ git branch -d testbranch
    ```

2017/01/02

1. Create this file with git command.
 - New git commands:
    - Initial Setup
    ```bash
    $ git config --global user.name "mike-r155"
    $ git config --global user.email mike_everything@hotmail.com
    $ git config --list
    $ git config --global core.autocrlf true
    ```

    - Add new file to new repository
    ```bash
    $ git init
    $ git add ./hisotry.md
    $ git commit -m "First commit." -m "2 line commit on command line."
    $ git remote add origin https://github.com/mike-r155/edu-git.git
    $ git push -u origin master
    ```

    - Add changed file and check it
    ```bash
    $ git diff
    $ git add -A
    $ git status
    ```

    - Reset an added file
    ```bash
    $ git reset HEAD ./history.md
    ```

2016/12/29

1. Install git on msys2 using [here](https://opcdiary.net/?p=29536) for reference

# What I want to learn

## Git commands
- [x] How to branch
- [x] How to change comments that I push
- [ ] How to send pull-request
- [ ] How to revert
- [ ] How to stash