## Docker service

```sh
/etc/rc.d/rc.docker [command]
```
Available commands: start stop restart status

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