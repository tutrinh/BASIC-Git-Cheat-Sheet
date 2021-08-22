---
description: Collection of git commands I used daily.
---

# Git Cheat Sheet

## Get Current Remote Repo
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

### New Branch Based on Existing One
```text
$ git branch <new-branch> <base-branch>
```
### New Branch from a Specific Commit
```text
$ git branch <new-branch> f71ac24d
```
### New Branch from a Remote Branch
```text
$ git checkout --track origin/<base-branch>
```
### New Branch in a Remote Directory
```text
$ git push -u origin <local-branch>
```
The "-u" create the upstream to the remote.


 

