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
echo "hi" > test.txt

# Add file → A (Added) 
git add test.txt

# Edit file → M (Modified)
echo "hello" > test.txt

# Add again → A (Added)
git add test.txt

# Save → Clean
git commit -m "saved test file"
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