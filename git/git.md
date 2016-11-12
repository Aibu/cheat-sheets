## Rename local or remote branch

### Rename a local branch
If in the same branch
```
git branch -m new-name
```
If in a different branch
```
git branch -m old-name new-name
```

### Rename a remote branch
```
git push origin :old-name new-name
```
The command above will delete the old branch and push the renamed branch to remote. 


