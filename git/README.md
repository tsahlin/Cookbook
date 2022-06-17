# Git

### Revert a commit and leave the reverted files as staged changes
```bash
git revert -n <commit>
```

### Show number of commits per author
```bash
git shortlog -sn

# Exclude merge commits
git shortlog -sn --no-merges

# Count from a specific date
git shortlog -sn --no-merges --since "01 January 2021"
```
