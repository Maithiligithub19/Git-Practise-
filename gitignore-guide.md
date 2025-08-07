# .gitignore Guide

## What is .gitignore?

A file that tells Git to ignore certain files.

## Why use it?
- Hide private files
- Skip junk files  
- Don't save big files

## How to make one?
1. Create file named ".gitignore"
2. Add file names you want to ignore
3. Save it

## Common things to ignore:
```
*.log        # log files
*.tmp        # temp files
node_modules # big folders
.DS_Store    # Mac junk
config.txt   # private stuff
```

## Example .gitignore file:
```
# My ignored files
*.log
*.tmp
private.txt
```