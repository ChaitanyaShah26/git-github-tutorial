# Git & GitHub Commands Cheatsheet 📋

## ⚙️ Setup & Configuration
Set your name for all commits:
```bash
git config --global user.name "[name]"
```
Set your email for all commits:
```bash
git config --global user.email "[email]"
```
Set the default branch name to 'main':
```bash
git config --global init.defaultBranch main
``` 

## 🚀 Starting a Project
Initialize a new local Git repository:
```bash
git init
```
Clone an existing repository from a URL to your local machine:
```bash
git clone [url]
```

## 💾 Making & Saving Changes
Show the status of changes as untracked, modified, or staged:
```bash
git status
```
Add a specific file to the staging area:
```bash
git add [file]
```
Add all new and modified files to the staging area:
```bash
git add .
```
Commit your staged changes with a descriptive message:
```bash
git commit -m "[message]"
```
View the commit history:
```bash
git log
```

## 🌱 Branches
List all local branches:
```bash
git branch
```
Create a new branch:
```bash
git branch [branch-name]
```
Switch to a different branch:
```bash
git checkout [branch-name]
```
Create a new branch and switch to it immediately:
```bash
git checkout -b [branch-name]
```
Merge the specified branch’s history into the current one:
```bash
git merge [branch]
```
Delete a local branch:
```bash
git branch -d [branch-name]
```

## 🌐 Syncing with Remotes
List all remote repositories:
```bash
git remote -v
```
Add a new remote repository:
```bash
git remote add origin [url]
```
Download all history from a remote repository without merging:
```bash
git fetch [remote]
```
Fetch and merge changes from the current branch's remote counterpart:
```bash
git pull
```
Push a specific branch to the 'origin' remote:
```bash
git push origin [branch]
```

## 📦 Stashing
Temporarily save modified, tracked files in order to switch branches:
```bash
git stash
```
Apply the most recent stash and remove it from the list:
```bash
git stash pop
```
List all stashed changesets:
```bash
git stash list
```
Discard the most recent stash:
```bash
git stash drop
```

## ⏪ Undoing Things
Unstage a file, but preserve its contents in the working directory:
```bash
git reset [file]
```
Discard all local changes in a specific file:
```bash
git checkout -- [file]
```
Create a new commit that undoes the changes from a specified commit:
```bash
git revert [commit-hash]
```
