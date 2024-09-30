# git-commands-notes

 1. `git status` is used to list all new or modified files that haven't yet been committed
```shell
git status
```
 2. `git add <file-name>` to update what will be committed or staged
```shell
# stage a single file, or multile files by separating file names by comma
git add <file-name>
git add <file1>,<file2>

# stage all changes at once shot
git add *
```
4. `git commit -m "write commit message"` is used to commit changes
```shell
git commit -m "write commit message"
```
5. `git push origin main` is used to push the project to GitHub main branch
```shell
git push origin main
```
6. `git branch` shows branches present in this repository
```shell
git branch
```
7. `git clone <url> <new-folder-name>` used to clone the project
```shell
# clone master branch to local
git clone <url> <new-folder-name>

# clone a perticular branch to local
git clone -b <branch> <repo-url> <new-folder-name>
```
8. `git branch <new-branch-name>` used to create new branch
```shell
git branch <new-branch-name>
```
9. `git checkout <branch-name>` used to switch from one branch to another branch
```shell
# switch to existing branch
git checkout <branch-name>

# create new branch and switch to it
git checkout -b <branch-name>
```
10. `git diff` compare the changes
```shell
git diff
```
11. Use git stash when you want to record the current state of the working directory and the index, but want to go back to a clean working directory.
    https://git-scm.com/docs/git-stash
```bash
# push the intermediate changes with index reference
git stash

# push the intermediate changes with a message
git stash push -m "message to temp save"

# to check for all the stashes
git stash list

# to load a perticular changes use index to load
git stash apply <stash-index>

# to remove a stash with an index
git stash drop <stash-index>

# need to check what is it
git stash clear
```
