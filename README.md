# Git Cheat Sheet

## Configure Git

`git config --global user.name "[first name second name]"`

Sets the first name and the second name you want attached to your commits transactions

`git config --global user.email "[email address]"`

Sets the email address you want attached to your commits transactions


## Create repositories

`git init`

Creates a new local repository in the current directory

`git init [project name]`

Creates a new local repository with the specified project name

`git clone [project url]`

Downloads a project and its entire version history

`git clone [project url] [project name]`

Downloads a project and its entire version history with the specified project name


## Make changes

`git status`

Lists all new or modified files to be commited

`git add [file name]`

Snapshots the file in preparation for versioning

`git commit -m "[descriptive message]"`

Records the snapshots permanently in version history


## Group changes

`git branch`

Lists all local branches in the current directory

`git branch [branch-name]`

Creates a new branch with the specified branch name

`git checkout -b [branch-name]`

Creates a new branch with the specified branch name and switches to the specified branch and updates the working directory

`git checkout [branch-name]`

Switches to the specified branch and updates the working directory

`git merge [branch-name]`

Combines the specified branch's history into the current branch

`git branch -d [branch-name]`

Deletes the specified branch


## Review changes

`git diff`

Shows the differences not yet staged

`git diff [file name]`

Shows the differences not yet staged for a file

`git diff --staged`

Shows the differences between staging and the last file version

`git diff --staged [file name]`

Shows the differences between staging and the last file version for a file

`git diff [branch-name] [branch-name]`

Shows content differences between two branches

`git log`

Lists version history for the current branch

`git show [commit]`

Outputs metadata and content changes of the specified commit


## Redo changes

`git rm [file name]`

Deletes the file from the working directory and stages the deletion

`git rm --cached [file name]`

Removes the file from version control but preserves the file locally

`git reset [file name]`

Unstages the file, but preserves its contents

`git reset [commit]`

Undoes all commits after commit, preserving changes locally

`git reset --hard [commit]`

Discards all history changes back to the specified commit


## Synchronize changes

`git fetch`

Downloads all history from the repository

`git merge`

Combines branch into current local branch

`git pull`

Downloads history and incorporates changes

`git pull --rebase`

Downloads history and incorporates changes on the top of remote changes

`git push`

Uploads all local branch commits


## Temporary changes

`git stash`

Temporarily stores all modified tracking files

`git stash [descriptive message]`

Saves local modifications to a new stash

`git stash list`

Lists all stashed changesets

`git stash show`

Show the changes recorded in the stash

`git stash drop`

Discards the most recently stashed changesets

`git stash pop`

Restores the most recently stashed files