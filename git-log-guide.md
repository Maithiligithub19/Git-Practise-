# Git Log - See History

## What is git log?
Shows history of all your saves (commits).

## Two ways to use:

### 1. git log
Shows full details of each save.

```bash
git log
```

**What you see:**
- Commit ID (long number)
- Your name and email
- Date and time
- Your save message

### 2. git log --oneline
Shows short version - one line per save.

```bash
git log --oneline
```

**What you see:**
- Short commit ID
- Your save message only

## Example:

**Full version:**
```
commit 5fda014a1b2c3d4e5f6g7h8i9j0k
Author: Maithiligithub19 <email@example.com>
Date: Mon Jan 15 10:30:00 2024
    
    first commit
```

**Short version:**
```
5fda014 first commit
```

## When to use:
- `git log` - When you need full details
- `git log --oneline` - When you want quick overview

## Tip:
Press 'q' to exit the log view.