# Working with Remote Branches

## Push Local Branch to Remote
```sh
git push origin <branch_name>           # Push local branch to remote
git push -u origin <branch_name>        # Push and set upstream tracking
```

## Switch to a Remote Branch
```sh
git fetch origin                        # Fetch latest branches from remote
git switch <remote_branch>              # Switch to a remote branch (if already tracked)
git checkout -b <branch_name> origin/<branch_name>  # Create and switch to a local branch tracking remote
```

## List Remote Branches
```sh
git branch -r                           # List all remote branches
```

## Delete Remote Branch
```sh
git push origin --delete <branch_name>  # Delete a branch from remote
```
or 

# Initialize a Git Repository
```sh
git init                   # Initialize a new Git repository
```

# Check Repository Status
```sh
git status                 # Show the working tree status
```

# Add Files to Staging Area
```sh
git add .                  # Stage all changes
git add <file1> <file2>    # Stage specific files
```

# Commit Changes
```sh
git commit -m "Message"    # Commit staged changes with a message
```

# View Commit History
```sh
git log --oneline          # Show a summarized commit history
git log                    # Show detailed commit history
```

# View Differences
```sh
git diff                   # Show unstaged changes
git diff --staged          # Show staged changes
git diff <commit1> <commit2> # Show diff between two commits
```

# Basic Workflow Example
1. Initialize repository: `git init`
2. Check status: `git status`
3. Add files: `git add .` or `git add <file>`
4. Commit: `git commit -m "Initial commit"`
5. View log: `git log --oneline`
6. View changes: `git diff`

