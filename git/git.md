### Show all remote branches
```
git fetch origin
git checkout -v -a
git checkout -b <local-name> origin/<remote-name>
```
### Delete branches
```
git branch -d <branch-name>
Force delete
git branch -D <branch-name>
```

### Show commit tree
```
git log --graph
```

### Reset local repository (OVERWRITES local changes)
```
git reset --hard origin/<branch-name>
```

### Go back of one commit and reset remote branch
```
git reset --hard [previous Commit SHA id here]
git push origin <branch-name> -f
```

### Pull git repository to local/server empty folder
```
git init
git remote add origin git@github.com:me/<name>.git
git pull origin master
```

### Check remote repository
```
git remote -v
```

## Rename local or remote branch

### Rename a local branch
If in the same branch:
```
git branch -m new-name
```
If in a different branch:
```
git branch -m <old-name> <new-name>
```

### Rename a remote branch
```
git push origin :<old-name> <new-name>
```
The command above will delete the old branch and push the renamed branch to remote. 

[Go back to the Cheat Sheet menu.](../README.md)
