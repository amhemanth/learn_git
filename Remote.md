# Git Remote Repository Commands

## What is a Remote Repository?
A remote repository is a version of your project that is hosted on the Internet or network somewhere. You can push to, pull from, and sync with remotes like GitHub, GitLab, or Bitbucket.

## Add a Remote Repository
```sh
git remote add origin <url>         # Add a remote repository named 'origin'
```

## View Remote Repositories
```sh
git remote -v                      # List all remotes and their URLs
```

## Change Remote URL
```sh
git remote set-url origin <url>     # Change the URL of the remote named 'origin'
```

## Remove a Remote
```sh
git remote remove <name>            # Remove a remote repository
```

## Fetch and Pull from Remote
```sh
git fetch origin                    # Fetch changes from remote (does not merge)
git pull origin <branch>            # Fetch and merge changes from remote branch
```

## Push to Remote
```sh
git push origin <branch>            # Push local branch to remote
```

## Rename a Remote
```sh
git remote rename <old> <new>       # Rename a remote
```

## Show Remote Details
```sh
git remote show origin              # Show detailed info about the remote 'origin'
```
