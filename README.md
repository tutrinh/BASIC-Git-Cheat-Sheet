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

#### Add Changed files to Staging Area
Stages all files, including new, modified, and deleted files, including files in the current directory and in higher directories that still belong to the same git repository.
```text
$ git add -A
```

#### Resetting Changed Files from Staging Back To Local
Simply undoing the `git add`.
To undo `git add`, use `git reset`.
```text
$ git rest HEAD
```

## Commits
Committing changed files you want to push to staging area.
Commits are the building blocks of "save points" within Git's version control.
```text
git commit -m "update the README.md with link to contributing guide"
```

## Pushing Files to Remote Branch
- `$ git push -u origin master` command used when pushing a branch for the first time. This will configure the relationship between the remote and your local repository so that you can use `git push` and `git pull` with no addition options.
- `$ git push` command to push commit files to remote branch

## Pulling Files from Remote Branch
- `$ git pull`, pull files from remote branch to your local branch

## Reset Currrent Local Branch With Remote Branch
```text
git fetch
git reset --hard @{u} git reset --hard <branch-name>
```

## Difference Between Git Pull and Git Fetch
- `git fetch` tells local git to retreive the latest metadata info from the original. Does not do file transferring.
- `git pull` will make changes to your local files.

Use `git fecth` to know the changes done in the remote repo/branch since the last pull. Useful to know the differences before doing a `git pull` which will overwrite your local files in your current branch and working copy.
```text
git fetch
git diff ...origin
```

 

