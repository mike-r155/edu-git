# History
This is my learning history.


## Purpose
- Learning Android Modern Programming
- Learning Github
- Learning Git commands
- Learning English


## What I learned
2017/01/02
1. Push to Github with Android Studio.
 - Sign up for Github.
 - Repository is [here](https://github.com/mike-r155/edu-1).
  Note:
    - Do **NOT** create repository before you push from "VCS > Import into Version Control > Share project on GitHub"
    - If you have already done it, use "VCS > Git... > Push Commits > origin : master"
2. Create this file with git command.

New git commands:

 - Initial Setup
```
- git config --global user.name "mike-r155"
- git config --global user.email mike_everything@hotmail.com
- git config --global core.editor
- git config --list
- git config --global core.autocrlf true
```

 - Add new file to new repository
```
- git init
- git add ./hisotry.md
- git commit -m "First commit." -m "2 line commit on command line."
- git remote add origin https://github.com/mike-r155/edu-git.git
- git push -u origin master
```

 - Add changed file and check it
```
- git diff
- git add -A
- git status
```

 - Revert it
```
- git reset HEAD ./history.md
```

2016/12/29 Install Android Studio from [learning web page](http://dotinstall.com/lessons/basic_android_v2).


# What I want to Learn
## git commands
- How to branch
- How to revert
- How to change comments that I push
