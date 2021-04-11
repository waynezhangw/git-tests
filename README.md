# Git-practice

For testing:

git filter-branch

```shell
git filter-branch --force --index-filter \
  "git rm --cached --ignore-unmatch PATH-TO-YOUR-FILE-WITH-SENSITIVE-DATA" \
  --prune-empty --tag-name-filter cat -- --all
```

BFG Repo-Cleaner

```shell
bfg --delete-files YOUR-FILE-WITH-SENSITIVE-DATA
```

