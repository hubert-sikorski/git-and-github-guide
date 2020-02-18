![Git&GitHub](img/git&github-guide.png)

## [Wiki](https://github.com/princeelector/git-and-github-guide/wiki)

## Table of contents

- [Git commands](#git-commands)
  - [User configuration](#user-configuration)
  - [Repository setup](#repository-setup)
  - [Inspect & Compare](#inspect--compare)
  - [Tracking path changes](#tracking-path-changes)
  - [Staging & Snapshot](#staging--snapshot)
  - [Branches & Merging](#branches--merging)
  - [Share & Update](#share--update)
  - [Rewrite history](#rewrite-history)
  - [Temporary commits](#temporary-commits)
- [Git workflow](#git-workflow)
- [Ignoring files](#ignoring-files)
- [Committing guideline](#committing-guideline)
- [Using GitHub](#using-github)

# Git commands

## User configuration

- `git config --global user.name '[firstname lastname]'` - Set a name for identification. Hint: You can use `-g` flag instead of `--global`

- `git config -g user.email '[valid-email]'` - Set associated email address.

- `git config -g color.ui auto` - Set automatic command line coloring for Git for easy reviewing.

## Repository setup

- `git init` - Initialize an existing directory as a Git repository.

- `git clone [url]` - Retrieve an entire repository from a hosted location via URL.

## Inspect & Compare

- `git log` - Show the commit history for the currently active branch.

- `git log branchB..branchA` - Show the commits on branchA that are not on branchB.

- `git log --follow [file]` - Show the commits that changed file, even across renames.

- `git diff branchB..branchA` - Show diff of what is in branchA that is not in branchB.

- `git show [SHA]` - Show any object in Git in human-readable format.

## Tracking path changes

- `git rm [file]` - Delete the file from project and stage the removal for commit.

- `git mv [existing-path] [new-path]` - Change an existing file path and stage the move.

- `git log --stat -M` - Show all commit logs with indication of any paths that moved.

## Staging & Snapshot

- `git status` - Show modified files in working directory, staged for next commit.

- `git add [file]` - Add a file as it looks now to staging area for your next commit. Use `git add .` to add all files.

- `git reset [file]` - Unstage a file while retaining changes in working directory.

- `git diff` - Difference of what is changed but not staged.

- `git diff --staged` - Difference of what is staged but not yet committed.

- `git commit -m [commit message]` - Commit your staged content as a new commit snapshot.

## Branches & Merging

- `git branch` - List your branches. a* will appear next to currently active branch.

- `git branch [branch name]` - Create a new branch at the current commit.

- `git checkout [branch name]` - Switch to another branch and check it out into your working directory.

- `git merge [branch]` - Merge the specified branch's history into the current one.

- `git log` - Show all commits in the current branch's history.

## Share & Update

- `git remote add [alias] [url]` - add a git URL as an alias.

- `git fetch [alias]` - fetch down all the branches from that Git remote.

- `git merge [alias]/[branch]` - Merge a remote branch into your current branch to bring it up to date.

- `git push [alias] [branch]` - Transmit local branch commits to the remote repository branch.

- `git push --force` - Overwrite remote repository with local working directory.

- `git pull` - Fetch and merge any commits from the tracking remote branch.

## Rewrite history

- `git rebase [branch]` - Apply any commits of current branch ahead of specified one.

- `git reset --hard [commit]` - Clear staging area, rewrite working tree from specified commit.

- `git rm --cached [file]` - Stop tracking specified file.

## Temporary commits

- `git stash` - Save modified and staged changes.

- `git stash list` - List stack-order of stashed file changes.

- `git stash pop` - Write working from top of stash stack.

- `git stash drop` - Discard the changes from top of stash stack.

# Git workflow

# Ignoring files

# Committing guideline

# Using GitHub
