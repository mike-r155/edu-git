# Git History
This is my history of learning about git.


## Purpose
- Learning Github
- Learning Git commands
- Learning English


## What I learned

2017/01/04

1. Create branch and marge it.

New git commands:

 - Create branch
```bash
$ git branch
$ git testbranch
$ git checkout testbranch
```

 - Marge to master
```bash

```

2017/01/02

1. Create this file with git command.

New git commands:

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

2016/12/29 Install git on msys2 using [here](https://opcdiary.net/?p=29536) for reference

# What I want to learn

## Git commands
- [x] How to branch
- [ ] How to revert
- [ ] How to change comments that I push
