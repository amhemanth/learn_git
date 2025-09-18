# Git Rebase Commands

## What is Git Rebase?
Rebasing is a way to move or combine a sequence of commits to a new base commit. It is often used to keep a clean, linear project history.

## Basic Rebase Commands
```sh
git rebase <branch>                # Rebase current branch onto another branch
git rebase origin/main             # Rebase onto the latest main branch from remote
```

## Interactive Rebase
```sh
git rebase -i <commit_hash>        # Start an interactive rebase from a specific commit
```

## Continue, Skip, or Abort a Rebase
```sh
git rebase --continue              # Continue after resolving conflicts
git rebase --skip                  # Skip the current commit during a rebase
git rebase --abort                 # Abort the rebase and return to the original branch
```

## Example: Rebase Feature onto Main
```sh
git checkout feature-branch
git rebase main
```

## Tips
- Use rebase to keep your feature branch up to date with main before merging.
- Prefer rebase for a linear history, but be careful when rebasing shared branches.
