# Git Workflow - Simple Guide

## The Flow
```
Your Files → Ready Box → Saved → GitHub
     |          |         |        |
  [Edit]   [git add]  [commit]  [push]
```

## Steps
1. **Edit files** - Change your files normally
2. **Get ready** - `git add .` (put in ready box)
3. **Save** - `git commit -m "message"` (take picture)
4. **Upload** - `git push` (send to GitHub)

## Example
```bash
# 1. Edit files
echo "Hello" > file.txt

# 2. Get ready
git add .

# 3. Save
git commit -m "added hello file"

# 4. Upload
git push
```

Think: Write → Package → Mail → Deliver