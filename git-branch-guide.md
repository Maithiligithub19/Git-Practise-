# Git Branches - Simple Guide

## Basic Commands:

### See branches
```bash
git branch
```

### Create branch
```bash
git branch feature-name
```

### Switch branch
```bash
git switch branch-name
```

### Create and switch
```bash
git switch -c new-branch
```

### Delete branch
```bash
git branch -d branch-name    # Safe delete
git branch -D branch-name    # Force delete
```

### Merge branch
```bash
git switch main              # Go to main branch
git merge feature-name       # Merge feature into main
```

## Quick Example:
```bash
git switch -c login          # Create and switch
git add .
git commit -m "added login"
git switch main              # Go back to main
git merge login              # Merge login into main
git branch -d login          # Delete when done
```

## Remember:
- Work on features in separate branches
- Switch to main before creating new branches
- Delete branches when finished