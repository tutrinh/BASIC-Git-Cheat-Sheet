---
description: Collection of git commands I used daily.
---

# Git Cheat Sheet

#### Git Status
```text
$ git status
```
`git status` show the current state of the working directory and staging area.
- List changed files in current directory that have not yet been committed
- If changed files are staged or not
- If current local branch is linked to a remote branch, will tell if local branch is behind or ahead by any commits.

#### Get Current Remote Repo
```text
$ git remove -v
```
## Branch
#### Show Branches
```text
$ git branch
```
#### New Branch Based on the Current HEAD
```text
$ git branch <new-branch>
```

#### New Branch Based on Existing One
```text
$ git branch <new-branch> <base-branch>
```
#### New Branch from a Specific Commit
```text
$ git branch <new-branch> f71ac24d
```
#### New Branch from a Remote Branch
```text
$ git checkout --track origin/<base-branch>
```
#### New Branch in a Remote Directory
```text
$ git push -u origin <local-branch>
```
The "-u" create the upstream to the remote.

## Add Files to Commit

## Commits

## Pushing Files to Remote Branch
- `$ git push -u origin master` command used when pushing a branch for the first time. This will configure the relationship between the remote and your local repository so that you can use `git push` and `git pull` with no addition options.
- `$ git push` command to push commit files to remote branch

## Pulling Files from Remote Branch
- `$ git pull`, pull files from remote branch to your local branch





 

