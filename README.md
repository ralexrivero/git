# Git and Github

## Environment

- `ubuntu`
- `bash`
- `vim`
- `VS Code`
- `git`
- `github`

## Commands

### basics

`git status` see the status of the branch, tracked, untracked, commited, changed files
`git diff` see differences in files
`git diff --staged` see differences in staged files
`git add .` to add all the changes in the current branch to the stage area
`git commit -m "comment"` commit staged changes
`git commit -a -m "comment"` direc commit skipping the stage area

### branch

`git branch` see the branches an star the actual branch
`git branch <name>` create the named branch
`git checkout <name>` change to the named branch
`git branch -v` show branches and commit

### see branch log

`git log`
> branch in one line
`git log --online`
> graph representation to see devergent branch
`git log --online --graph --all`

### Branching workflow in production

- Long running branches (long term)
  - Master
  - Development
- Topic branches (short term)
  - Authentication
  - UI changes

### Rebasing

> checkout the branch where commits will be rebased from
`git checkout <branch>`
`git rebase master`
`git checkout master`
`git merge <branch>` merge the branch into master with fast forward strategy

both branches are at the same point

### Misc commands

> show commit detail

`git log`
`git show <commit hash>`

> stashing (changes not ready to be commited yet, unfinish work, task don't complete, then saved in a stack for apply later)

`git stash` if the file is untracked is needed to be added to the stage area
`git stash list` to see the stack of stashed changes
`git stash apply stash@{0}` to apply the first stash or the number of the stash
`git stash drop stash@{0}` to drop the stash

> clean
`git clean -f -d` recursively delete directories and files, forced

> change the messege of the last commit
`git commit --amend` and modify the text in editor. Save changes

> change the last commit

Create changes, add them to the stage area, don't commit, and amend to add them to the last commit
`git commit --amend` and modify the text in editor. Save changes

> trying to change the last commit after pushing changes will cause a divergence

> switch
`git switch <commit_id>`
`git switch -` to go back to the last commit

> create new branch from the past with the new commits
`git switch -c <new_branch>` created from the checkout commit

> revert
`git revert <commit_it>` to undo the changes and preserve the commit

> reset
`git reset --soft <commit_id>` to undo the changes and preserve the commit
`git clean -f -d` after soft reset need to clean the files or stage and commit
`git resrt --hard <comit_id>` to undo the changes and delete the commit

## Author

> Ronald
<!-- twitter -->
[![Twitter](https://img.shields.io/twitter/follow/ralex_uy?style=social)](https://twitter.com/ralex_uy) <!-- linkedin --> [![Linkedin](https://img.shields.io/badge/LinkedIn-+24K-blue?style=social&logo=linkedin)](https://www.linkedin.com/in/ronald-rivero/) <!-- github --> [![Github](https://img.shields.io/github/followers/ralexrivero?style=social)](https://github.com/ralexrivero/) <!-- vagrant --> [![Vagrant](https://img.shields.io/static/v1?label=&message=Vagrant%20Profile&color=1868F2&logo=vagrant&labelColor=2F333A)](https://app.vagrantup.com/ralexrivero) <!-- docker --> [![Docker](https://img.shields.io/static/v1?label=&message=Docker%20Profile&color=2496ED&logo=Docker&labelColor=2F333A)](https://hub.docker.com/u/ralexrivero)
