# Git Cheat Sheet – Flavor Octocat

## General Overview of Git structure

![image](https://merely-useful.tech/py-rse/figures/git-cmdline/git-remote.png)

An overview of the ``git structure`` can be taken from the above picture. We can simply derive from it that there are 4 distinct blocks:
- working files: our local working directory
- staging area: the changes we want to add to our repository
- local repository: a local environment where we track all our file changes
- remote repository: a remote environment that can be available for other users

## Basic Commands

### Manipulating repositories

* ``git init``: Creates an empty Git repository on your local disk.
* ``git clone``: Creates a local copy of a remote Git repository. Requires HTTPS or SSH URL to clone from.
* ``git pull``: Updates a local copy of a remote Git repository.
* ``git checkout``: Switches to a different branch of a local Git repository. Can also be used to create new branches locally.
* ``git add``: Add a file within the directory structure of a local Git repository to version control.
* ``git commit``: Save currently untracked changes to a local Git repository.
* ``git push``: Updates a remote Git repository to match a local copy. Only works if no new commits have been made remotely on the same branch, else you must pull and merge/rebase first.


### Informative commands

* ``git status``: Display current untracked changes that can be committed.
* ``git log``: Display commits to a local Git repository in order of recency.
* ``git help``: Built-in help for Git commands - supply name of a particular command to learn about it.

## Git Cheat Sheet Octocat

[![CC BY 4.0][cc-by-shield]][cc-by]

A joint git cheat sheet as a training repository to learn git workflows

### Category: Branch, forks, merge/rebase

* ``git branch``: creates a new branch
* ``git checkout <branch-name>``: switch to the specified branch 
* ``git merge``: merges the changes of the remote branch to the local branch
* ``git rebase``: moving the base of a branch onto a different position
* ``git pull``: downloads and merges changes to your local repository
* ``git fetch``: make changes on the remote repository locally visible

![Diff Rebase Merge](images/git_commit_merge_rebase.png)

## Advanced Commands

* `git blame` : Show what revision and author last modified each line of a file
* `git reflog` : Manage reflog information (equivalent to `git relog show HEAD`)
* `git effort` (from `git-extras` repository) : Show effort statistics on file(s) in repository 
* `git commit -m "Title of commit" -d "Description of commit"` : to specify a commit message and description without going to vim
* `aheadfork` : find GitHub forks that are ahead
* `git stash` : Stash the changes in a dirty working directory away

