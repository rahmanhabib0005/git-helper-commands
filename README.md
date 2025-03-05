# Git Commands Cheat Sheet

## Initial Setup

```sh
# Set up global username and email
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

## Starting a Repository

```sh
# Initialize a new Git repository
git init

# Clone an existing repository
git clone <repository_url>
```

## Basic Commands

```sh
# Check the status of the working directory
git status

# Add files to the staging area
git add <file>       # Add a specific file
git add .           # Add all files

# Commit staged files with a message
git commit -m "Commit message"
```

## Branching and Merging

```sh
# List all branches
git branch

# Create a new branch
git branch <branch_name>

# Switch to a branch
git checkout <branch_name>

# Create and switch to a new branch
git checkout -b <branch_name>

# Merge a branch into the current branch
git merge <branch_name>
```

## Working with Remote Repositories

```sh
# Add a remote repository
git remote add origin <repository_url>

# Fetch changes from the remote repository
git fetch

# Pull the latest changes from the remote repository
git pull origin <branch_name>

# Push changes to the remote repository
git push origin <branch_name>
```

## Undoing Changes

```sh
# Unstage a file (undo `git add`)
git reset <file>

# Reset to the last committed state
git reset --hard

# Reset to the last committed state and set-top commit
git reset --hard Head

# Revert a commit
git revert <commit_hash>

#Remove untracked changes
git clean -fd

#Back to Previous commit
git reset --hard HEAD~1
```


## Stashing Changes

```sh
# Stash current changes
git stash

# List all stashes
git stash list

# Apply the latest stash
git stash apply

# Drop a specific stash
git stash drop stash@{n}
```

## Viewing History

```sh
# View commit history
git log

# View a compact commit history
git log --oneline --graph --decorate --all
```

## Tagging

```sh
# Create a new tag
git tag <tag_name>

# Push a tag to the remote repository
git push origin <tag_name>
```

## Advanced Commands

```sh
# Amend the last commit message
git commit --amend -m "New commit message"

# Rebase a branch
git rebase <branch_name>

# Cherry-pick a commit into the current branch
git cherry-pick <commit_hash>
```

## Deleting Branches

```sh
# Delete a local branch
git branch -d <branch_name>

# Delete a remote branch
git push origin --delete <branch_name>
```

## Cleaning Up

```sh
# Remove untracked files
git clean -f

# Remove untracked directories
git clean -fd
```

## Summary
This cheat sheet contains essential Git commands to help you manage your repositories efficiently.
