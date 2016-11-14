## Docker

### Install docker to server
```
wget -qO- https://get.docker.com | sh
```

### Start a docker container
```
docker run <container-name>
```

### Start a container in background mode
```
docker run -d <name-of-image>:<version-or-tag>
```

### Start a container in background mode and expose port to be accessed from the web
```
docker run -d -P <name-of-image>:<version>
```

### Remove all Docker containers
```
docker rm $(docker ps -aq)
docker rmi <node>
```

### Remove an image
```
docker ps
docker rmi <image-id>
```

### Inspect a container
```
docker inspect --format='{{json .NetworkSettings.Networks}}' <container-name>
```

### Log output of containers
```
docker logs tail -f
```

### List of all containers
```
docker ps
docker ps -a (all containers included those stopped)
```

### List all images present in the server
```
docker images
```

### Open terminal inside a container
```
docker run -i (stdin) -t (terminal) ubuntu(<name-of-image>):latest(<tag?) /bin/bash
```

### Exit the container without stopping it
```
Ctrl + p + q
```

### Open terminal within a running dock
```
docker exec -i -t <dockid> /bin/bash
```

### Open Mongo within a running dock
```
docker exec <dockid> mongo
```

[Go back to the Cheat Sheets menu.](../README.md)
