## Useful

#### Show running
```sh
docker ps
```

#### Stop all containers
```sh
docker stop $(docker ps -q)
```

#### Restart all containers
```sh
docker restart $(docker ps -aq)
```

#### Pull all new images
```sh
docker images | awk '{print $1":"$2}' | grep -v REPOSITORY | xargs -L1 docker pull 
```

## Docker containers

#### Basic commands

```sh
docker [command] [containername]
```
Available commands: start stop restart pause logs

#### Print all container names:

```sh
docker ps --format ‘{{.Names}}’
```
#### Print all container images:

```sh
docker ps --format ‘{{.Image}}’
```
