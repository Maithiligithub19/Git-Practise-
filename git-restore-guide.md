# Git Restore - Undo Changes

## What is git restore?
Brings back old version of files.

## Two types:

### 1. git restore filename
- Undo changes in working folder
- Gets back last saved version
- Use when you messed up a file

### 2. git restore --staged filename  
- Remove file from ready box
- File goes back to working folder
- Use when you added wrong file

## Examples:

```bash
# You changed file1.txt but want old version back
git restore file1.txt

# You added file2.txt but don't want to save it yet
git restore --staged file2.txt
```

## When to use:
- Made mistake in file → `git restore filename`
- Added wrong file → `git restore --staged filename`

## Warning: 
git restore deletes your changes forever!