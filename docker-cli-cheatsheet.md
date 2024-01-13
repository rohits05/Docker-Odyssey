# Docker CLI Cheatsheet

A quick reference guide for Docker CLI commands.

## Table of Contents

- [Introduction](#introduction)
- [Images](#images)
- [Containers](#containers)
- [Networks](#networks)
- [Volumes](#volumes)
- [Compose](#compose)
- [Swarm](#swarm)
- [Miscellaneous](#miscellaneous)

## Introduction

Docker is a powerful platform for developing, shipping, and running applications in containers. This cheatsheet covers essential Docker CLI commands.

## Images

### Pull an image from Docker Hub

```bash
docker pull image_name:tag
```

### List downloaded images

```bash
docker images
```

### Remove an image
```bash
docker rmi image_name:tag
```


## Containers

### Run a container
```bash
docker run image_name:tag
```

### List running containers
```bash
docker ps
```

### List all containers (including stopped)
```bash
docker ps -a
```

### Stop a running container
```bash
docker stop container_id
```

### Remove a container
```bash
docker rm container_id
```


## Networks

### Create a network
```bash
docker network create network_name
```

### List networks
```bash
docker network ls
```

### Remove a network
```bash
docker network rm network_name
```


## Volumes

### Create a volume
```bash
docker volume create volume_name
```

### List volumes
```bash
docker volume ls
```

### Remove a volume
```bash
docker volume rm volume_name
```


## Compose

### Run services defined in a Compose file
```bash
docker-compose up
```

### Stop services defined in a Compose file
```bash
docker-compose down
```


## Swarm

### Initialize a Swarm
```bash
docker swarm init
```

### Join a Swarm as a worker or manager
```bash
docker swarm join --token TOKEN IP:PORT
```

### Deploy a service in Swarm mode
```bash
docker service create --name service_name image_name:tag
```


## Miscellaneous

### View Docker version
```bash
docker version
```

### View system-wide information
```bash
docker info
```

### Access a shell inside a running container
```bash
docker exec -it container_id /bin/bash
```

## Happy Dockerizing! May your containers be lightweight, your deployments seamless, and your tech journey a continuous adventure. Keep exploring, learning, and pushing the boundaries of what's possible. Cheers to the knowledge seekers and tech enthusiasts around the GitHub universe! 🚀🐳