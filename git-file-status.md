# Git File Status - U, M, A

## What the Letters Mean

### U - Untracked
- New file Git doesn't know
- **Fix:** `git add filename`

### M - Modified  
- Changed existing file
- **Fix:** `git add filename`

### A - Added
- File ready to save
- **Fix:** `git commit -m "message"`

## Quick Example
```bash
# Create file → U (Untracked)
echo "Welcome to my project" > index.html

# Add file → A (Added) 
git add index.html

# Edit file → M (Modified)
echo "<h1>My Website</h1>" > index.html

# Add again → A (Added)
git add index.html

# Save → Clean
git commit -m "created website homepage"
```

## Remember
- **U** = Git doesn't know this file
- **M** = File changed, need to add
- **A** = Ready to save with commit

## Git Status Command

Shows what files changed in your project.

**When to use:**
- Before saving files
- To see what's different
- Check if everything is ready

**What it shows:**
- Red files = Need to add (git add)
- Green files = Ready to save (git commit)
- Nothing = All good, no changes

**Quick tip:** Always check git status before git commit