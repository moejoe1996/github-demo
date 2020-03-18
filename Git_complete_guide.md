# GIT COMPLETE GUIDE

# Source control?

    - Backup or versioning.
    - control de diferent changes from your files.
    - it allows collaboration
    - Blame
    - branching ot isolate changes
    - Code review

# who needs source control?

    - Software developers/engineers/ programmers
    - Freelancers
    - Web designers: Assets, pages, images
    - Graphic Artists
    - Anyone who wants to share the code

# Source Control Options

## Two types:

        - Centralized: Free, commercial, requires a conection to a server
        - Decentralized/ Distributed: Mercurial, git, most operations are local

# Why git?

    - Distributed source control system
    - Massively scales
    - Open source
    - very fast and free
    - Active commmunity
    - Most popular

# Terminology:

    - A **repository** contains files, history, config managed by git.
    - Thre states of Git:
        1. Working directory: Current working project.
        2. Staging Area: Holding area to queueing files to the repository
        3. Commit: sending the changes to the repository
    - Master Branch: branches contain commits

# Commands list

## Basics

    `pwd`: shows your current directory
    `mkdir`: create a new directory
    `mkdir -p <directories>`: creates varius folders with sub-folders
    `cd`: change directory
    `ls`: list all items in a directory
    `git clone <url>`: clone repository in a directory
    `git status`: shows the status of the current git project
    `git add <file>`: adds a file to be tracked by git (stages the file)
    `git add -A`: will add and update any changes to the working directory
    `git commit -m "<Messages>"`: Commits all of the files in the staging area
    `git push origin master`: sends the commited files to the remote repository.
    `git pull origin master`: pulls every change from the remote repository to local.
    `git commit -am "<message>"`: to stage and commit all in one command
    `git ls-files`: list of files that git is tracking in the current repository.
    `echo "<some text>">>example.txt`: to create a file with text using cmd
    `cat file.txt`: displays contents of file
    `unzip <path to file>`: unzips the file in current directory
    `mv <path to file> <new path>`: moves/renames file

## Staging

    - `git add <file>`: adds a file to the staging area
    - `git add .`: add everythong to the staging area

## Commiting and Pushing

    - `git commit -m "message"`: Commit command
    - `git push origin <branch>`: pushes the changes to the repository

## Setting your username and email

    - `git config --global user.name "yourname"`
    - `git config --global user.email "email@example.com"`
    - To confirm `git config --global --list`

## Recursive add

    `git add .`: add all files recursively in a directory

## Backing out changes

    `git reset HEAD <file>`: to unstage the file
    `git checkout -- <file>`: reverts the file to before the changes were made

## Renaming and Moving files

    `git mv <current file name> <new file name>`: to rename a file and git knows.
    `mv <current file> <new file>`: rename file at OS level. need to be added to the git again.
    `git add -A`: this way git will be aware.

## Deleting Files

    `rm <file>`: removes the file from the local system
    `git rm <file>`: removes a file that is beign tracked by git
    `git checkout -- <file>`: to discard changes in the working directory

## History

    `git log`: show the commit history in inverse chronological order.
    `git log --oneline --graph --decorate --all`: shows history in a nice way
    `git log --since="3 days ago"`: will bring the commits that happened in the last 3 days
    `git log -- <file>`: shows the commits that involves that file
    `git show <Commit id>`: shows the history of a commit

## Git Alias

    To set new aliasses. For example to set a new alias for the git log command:
        `git config --global alias.hist "<Full command without git>"`

    To modify the config file
        `code ~/.gitconfig`: it opens the config file to make changes.

## Ignoring Unwanted files and Folders

    This file will contain a expression per line with patterns that GIT will ignore.
    This file takes regex patterns to exclude files or specific files
    `code .gitignore`: to create the file which GIT will ignore

## Comparing Working directory and Git

    'git diff': shows the file with the changes made to that file
    'git difftool': launched the tool installed in the computer and shows the differences visualy
    `git diff HEAD`: compares the working directory with the repository
    `git diff --staged HEAD`: compares local to the last commit in the current branch.
    `git diff -- <file path>`: limits just to show the specified file.
    `git diff <refence 1> <reference 2>`:Compares two commits.
    `git diff master origin/master`:Compares local master branch and the remote master branch

## Branching Basics

    `git brach -a`: list all existing branches
    `git branch <name of branch>`: creates a new branch
    `git checkout <name of branch>`: switch to the desired branch
    `git branch -m <previous branch> <rename branch>`: to rename a branch
    `git branch -d <name of branch>`: to delete a branch
    `git checkout -b <new branch>`: to create and checkout new branch
    `git merge <branch-to-merge>`: merges the branch into your current branch
    ### Fast Foward

        FAST FORWARD: when you make changes only to the branch and none to master. A fast foward merge will take place. Meaning that it will put all the changes in front of the master branch as if there was only one branch.

    ### Disable Fast Foward
