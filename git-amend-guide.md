# Git Amend - Fix Last Commit

## What is git amend?
Changes your last commit without creating a new one.

## Basic Command:
```bash
git commit --amend
```

## Common Uses:

### Fix commit message
```bash
git commit --amend -m "new message"
```

### Add forgotten files
```bash
git add forgotten-file.txt
git commit --amend --no-edit
```

### Change files and message
```bash
git add .
git commit --amend -m "updated message"
```

## Example:
```bash
# Made a commit with typo
git commit -m "added logn feature"

# Fix the message
git commit --amend -m "added login feature"

# Or forgot to add a file
git add missing-file.txt
git commit --amend --no-edit
```

## Flags:
- `--no-edit` - Keep same message
- `-m "message"` - Change message

## Warning:
Only amend commits that haven't been pushed yet!