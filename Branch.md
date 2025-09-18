
# Git Branching Commands

## Create a New Branch
```sh
git branch <branch_name>           # Create a new branch
git checkout -b <branch_name>      # Create and switch to the new branch
git switch -c <branch_name>        # Create and switch to the new branch (recommended)
```

## Switch Between Branches
```sh
git switch <branch_name>           # Switch to an existing branch (recommended)
git checkout <branch_name>         # Switch to an existing branch
```

## List Branches
```sh
git branch                        # List all local branches
git branch -a                     # List all branches (local and remote)
```

## Rename a Branch
```sh
git branch -m <new_name>          # Rename current branch
git branch -m <old> <new>         # Rename a specific branch
```

## Delete a Branch
```sh
git branch -d <branch_name>       # Delete a branch (safe, checks for unmerged changes)
git branch -D <branch_name>       # Force delete a branch
```

## Merge Branches
```sh
git merge <branch_name>           # Merge specified branch into current branch
```

## View Branch History
```sh
git log --oneline --graph --all   # Visualize branch history
```