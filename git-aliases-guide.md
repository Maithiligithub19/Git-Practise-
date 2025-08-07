# Git Shortcuts

## Two ways to make shortcuts:

### Bash Shortcuts (All projects)
```bash
nano ~/.bashrc
```
Add these:
```bash
alias gs='git status'
alias ga='git add .'
alias gc='git commit -m'
alias gp='git push'
```
Save and run:
```bash
source ~/.bashrc
```

### Git Shortcuts (One project)
```bash
git config alias.st status
git config alias.cm commit
git config alias.lg "log --oneline"
```

## How to use:
```bash
# Bash shortcuts (no 'git')
gs
ga
gc "my message"

# Git shortcuts (need 'git')
git st
git lg
```

## See all shortcuts:
```bash
git config --list | grep alias
```