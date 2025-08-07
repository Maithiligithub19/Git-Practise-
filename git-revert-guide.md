# Git Revert - Undo Old Saves

## What is git revert?
Undoes an old save (commit) by creating a new save that cancels it out.

## How it works:
- Doesn't delete the old save
- Creates a new save that undoes the changes
- Safe way to fix mistakes

## How to use:

### Step 1: Find the commit ID
```bash
git log --oneline
```

### Step 2: Revert that commit
```bash
git revert [commit-id]
```

## Example:
```bash
# See history
git log --oneline
5fda014 added bug
3abc123 first commit

# Undo the "added bug" commit
git revert 5fda014
```

## What happens:
1. Git creates a new commit
2. This new commit removes the changes from the old commit
3. Your history stays complete

## When to use:
- Fix mistakes in old saves
- Undo changes safely
- When working with others (safer than deleting)

## Note:
Git will ask you to write a message for the revert commit.