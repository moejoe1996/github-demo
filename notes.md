# LEARN GIT IN 15 MINUTES

## What is GIT?

    - Distributed version control system (VCS)
    - Is used to track changes in a project files.

## REPOSITORIES

    - These are the containers for GIT
    - to use GIT, every time you need to initialize a repository.

## GIT INITIALIZATION COMMAND

    - In an empty folder, if I want to track changes in that folder just run: `git init`

## CHECKING GIT STATUS

    - The command is: `git status`
    - It shows the "Status" of your current repository. shows the commits,
    branches, etc.

## STAGING AND COMMITS

    - Firs we need to stage project files and then commit
    - To stage we need to use: `git add file.js`
    - To add multiple files: `git add file.js file2.js file3.js`
    - To add all changes into the staging area: `git add .`
    - Finally, to commit we use: `git commit -m "Commit message"`
    ______________________________________________________________
    - Return to a previous commit: `git checkout <commit-hash>`

## LOGGING

    - To show a history of the changes made you can type: `git log`

## BRANCHING

- A branch in git is like a timeline of the repository.
- run: `git branch <new-branch-name>`
- To list all branches: `git branch`

---

- To merge a branch into the main project timeline (master): `git merge <branch-name>`
