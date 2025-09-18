# Git Merge Commands

## What is Git Merge?
Merging in Git combines changes from one branch into another. It's commonly used to integrate feature branches into the main branch.

## Basic Merge Commands
```sh
git merge <branch_name>           # Merge the specified branch into the current branch
git merge --no-ff <branch_name>   # Create a merge commit even if a fast-forward is possible
```

## Abort a Merge
```sh
git merge --abort                 # Abort the current merge process and revert to the pre-merge state
```

## Resolve Merge Conflicts
- Open conflicted files and edit to resolve conflicts.
- After resolving, mark as resolved:
```sh
git add <file>
git commit                       # Complete the merge after resolving conflicts
```

## View Merge History
```sh
git log --oneline --graph --all   # Visualize branch and merge history
```

## Tips
- Always pull the latest changes before merging: `git pull`
- Use `git status` to check for conflicts or staged changes during a merge.
