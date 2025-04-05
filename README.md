# Git Cheat Sheet

Tired of sacrificing brain cells (and tokens) chasing StackOverflow scrolls...hence

[1 Pulling a Single Branch](#pulling-a-single-branch)  
[2 Shallow Pull](#shallow-pull)  
[3 Cleaning Files After Modifying `.gitignore`](#cleaning-files-after-modifying-gitignore)  
[4 Managing Submodules](#managing-submodules)  
[4 Managing Branches](#managing-branches)

## Pulling a Single Branch
```bash
git clone --branch <branchname> --single-branch <repository-url>
```

## Shallow Pull
```bash
git clone --depth 1 <repository-url>
```

## Cleaning Files After Modifying `.gitignore`
```bash
git rm -r --cached .
git add .
git commit -m "Clean up ignored files"
```
## Managing Submodules

### Adding
```bash
git submodule add <repository-url> <path>
git commit -m "Add submodule"
```

### Updating
```bash

git submodule update --remote --merge
```
## Managing Branches

### Deleting Remote Branch
```bash
git push origin --delete <branchname>
```
