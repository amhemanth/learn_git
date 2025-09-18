# Git Stash Commands

## What is Git Stash?
Git stash temporarily shelves (or stashes) changes you've made to your working directory so you can work on something else, then come back and re-apply them later.

## Basic Stash Commands
```sh
git stash                  # Stash current changes (tracked files)
git stash -u               # Stash including untracked files
git stash -a               # Stash including all (untracked + ignored) files
```

## List Stashes
```sh
git stash list             # Show list of stashed changes
```

## Apply or Pop Stash
```sh
git stash apply            # Apply the latest stash (keeps stash in list)
git stash apply stash@{n}  # Apply a specific stash
git stash pop              # Apply and remove the latest stash
git stash pop stash@{n}    # Apply and remove a specific stash
```

## Drop or Clear Stash
```sh
git stash drop stash@{n}   # Remove a specific stash
git stash clear            # Remove all stashes
```

## Stash with Message
```sh
git stash save "message"   # Stash with a custom message (legacy, use git stash push -m)
git stash push -m "msg"    # Stash with a custom message (recommended)
```

## Show Stash Details
```sh
git stash show             # Show summary of latest stash
git stash show -p stash@{n}# Show full diff of a specific stash
```

## Create a Branch from Stash
```sh
git stash branch <branch_name> stash@{n} # Create and switch to a new branch from a stash
```
