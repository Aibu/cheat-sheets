# unix

### Create aliases
```
cd nano .bash_profile
alias name=‘command’
```

### Refresh bash
```
source ~/.bash_profile
```

### Copy local ssh key to clipboard 
```
cd ~/.ssh
cat id_rsa.pub | pbcopy
```

## USER

### Create user
```
adduser <username>
```

### Add to sudo group
```
adduser <username> sudo
```

### Get the list of users
```
cat /etc/passwd
```


## Transfer files betweeen servers

### Compress files: 
```
tar cvf <nomefile.tar> <filedazippare> <cartelladazippare>
```

### Connect to ftp server
```
ftp <www.nomeserver.it>
Send file to server
send <nomefile.tar>
```

### Retrieve file from server
```
ftp <www.nomeserver.it>
get <nomefile.tar>
```

### Unzip file 
```
tar unzip content without containing folder
tar xvf nomefile.tar
```

## Navigation
```
^A -> goes to the start of the line
^E -> goes to the end of the line
^U -> removes current line
pwd -> print working directory
￼cd -> goes to the user’s home directory
mv <source> <destination>
```

## COMPRESSION

### Compress bz2
```
tar cvjf <target>.tar.bz2 <sourcedir>/*
```

### SEARCH
```
find ./ -name nomefile.ext
```

### UTILITIES
Finds your current IP address
```
ifconfig | grep inet
```

[Go back to the Cheat Sheets menu.](../README.md)
