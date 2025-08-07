# Git Reset - Go Back in Time

## What is git reset?
Goes back to an old save and removes newer saves.

## Three types:

### 1. git reset --soft [commit-id]
- Goes back to old save
- Keeps your file changes
- Files stay in ready box (staged)

### 2. git reset --mixed [commit-id]
- Goes back to old save
- Keeps your file changes
- Files go back to working directory (unstaged)

### 3. git reset --hard [commit-id]  
- Goes back to old save
- Deletes all your file changes
- Everything goes back to that point

## How to use:

### Step 1: Find commit ID
```bash
git log --oneline
```

### Step 2: Reset to that commit
```bash
git reset --soft abc123    # Keep changes (staged)
git reset --mixed abc123   # Keep changes (unstaged)
git reset --hard abc123    # Delete changes
```

## Example:
```bash
# See history
git log --oneline
5fda014 bad commit
3abc123 good commit
1def456 first commit

# Go back to "good commit" - keep changes (staged)
git reset --soft 3abc123

# Go back to "good commit" - keep changes (unstaged)
git reset --mixed 3abc123

# Go back to "good commit" - delete everything
git reset --hard 3abc123
```

## When to use:
- **--soft** - Fix commit message or reorganize
- **--mixed** - Go back but keep working on files
- **--hard** - Start over from old point

## Warning:
--hard deletes your work forever! Be careful!