# __GitHub CheatSheet__

# User and Email Configuration

## Username Configuration
```powershell
git config --global user.name "<username here>"
```
## Email Configuration
```powershell
git config --global user.email "<your email>"
```
## To see the configuration
```powershell
git config --list
```
## To see the log files
```powershell
git log
```

# Basic Commands
## Initialize a repository as git repository
```powershell
git init
```
## Add files for staging
> To add all files
```powershell
git add .
```
> To add a single file
```powershell
git add <filename>
```
## Remove files from staging
> To remove all files from staging
```powershell
git remove .
```
> To remove a single file
```powershell
git remove <filename>
```
## Check the status of files
```powershell
git status
```
## Commit the changes
```powershell
git commit -m "initial commit"
```
## Adding the origin to push the files to the remote repository
```powershell
git remote add origin <https://<repo url...>
```
## Push the files to the remote repository
```powershell
git push -u origin master
```
## Pull the files from remote repository
```powershell
git pull
```
## Clone a remote repository
```powershell
git clone <url>
```
## To ignore files and directories that you don't want to push to the remote repository make .gitignore file and add files and directories name in that folder'
>For bash
```bash
touch .gitignore
```
>For poweshell
```powershell
new-item .gitignore
```
## To get the previous version of your files
>For single file
```powershell
git checkout <filename>
```
>For all files
```powershell
git checkout -f
```

---

##  SSH Key
> To generate ssh key
```powershell
generate ssh key

ssh-keygen -t rsa -b 4096 -C "shkr2209@gmail.com"
```
> To grep the ssh key
```powershell
cat <file path>
```
## To see the difference b/w old and new files
```powershell
git diff

git diff --staged
```
## To undo changes the files to the prior state
```powershell
git reset
```

# Advance Commands

## To see the last commits
`git log -p -<how many commits you want to see>`

## Branch Commands
```powershell
git branch

git merge

git rebase
```
> Command to resolve merge conflict
```bash
git log --merge

git diff

git checkout

git merge --abort

git reset --mixed

git reset
```

## To know the branches
`git branch`

## To create a new branch
`git branch <branch name>`

## To switch a branch
`git checkout <branch name>`

## To switch master branch
`git checkout master`

## To merge your branch into master branch
`git merge <branch name>`

## To create and switch a branch
`git checkout -b <branch name>`

## Merge Toolkit
```powershell
git mergetool

:wq
```

## To set url
`git remote set-url origin <your repo url>`
## To see url
`git remote -v`
## To push specific branch
`git push -u origin <branch name>`
