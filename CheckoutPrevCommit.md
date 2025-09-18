# Checking Out Previous Commits (HEAD~N)

Sometimes you may want to view or work with a previous state of your repository. `HEAD~2` refers to the commit two steps before the current commit (HEAD). This is useful for inspecting, testing, or creating a new branch from an earlier point in history.

## Example: Checkout to a Previous Commit
```sh
git checkout HEAD~2           # Move to the commit two steps before HEAD (detached HEAD state)
```

## Use Cases
- **Inspecting old code**: See what the project looked like at a previous commit.
- **Debugging**: Test or debug an issue that existed in an earlier commit.
- **Creating a branch from an old commit**:
    ```sh
    git checkout HEAD~2
    git checkout -b new-feature-from-old
    ```
    This creates a new branch starting from that previous commit.
