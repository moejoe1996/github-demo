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
    `cd`: change directory
    `ls`: list all items in a directory
    `git clone <url>`: clone repository in a directory
    `git status`: shows the status of the current git project
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
