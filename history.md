# History
This is my learning history.


## Purpose
- Learning Android Modern Programming
- Learning Github
- Learning Git commands
- Learning English


## What I learned
2017/01/03
1. Complete "Dot Install" android tutorial.
 - Create button and textarea.
 - Add code to change the text using the button.
 Note:
    - autocrlf setting makes line end character LF when you push to github.
    - Local changes dialog shows some files have different line end.
    - You can resolve the problem to pull files from github.

2. Next tutorial is on Github [mixi-inc](https://github.com/mixi-inc/AndroidTraining).
 - I notice that I have been developed android apps before, but I don't even know basic knowledge about android. I need to learn systematically about it.
 - Now, studying about sdk at practice of section 1-4.

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

 - Reset an added file
```
- git reset HEAD ./history.md
```

2016/12/29 Install Android Studio from [learning web page](http://dotinstall.com/lessons/basic_android_v2).


# What I want to learn

## Android programming
- How to use O-Auth
- How to use gradle script

## Git commands
- How to branch
- How to revert
- How to change comments that I push
