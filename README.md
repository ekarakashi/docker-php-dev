# docker-php-dev

## Introduction
This is a Docker Compose project used to build a container image for nginx and php-fpm with mysql.
The aim is to provision a developer environment with no effort in a very short time, while 
also experimenting a bit with docker. 
In this implementation, I use PHP 5.6.x, MySql:latest, Nginx:latest

## Prerequisites
[Install Docker Compose tool.](https://docs.docker.com/compose/install/) 

## Runn/Stop
To build and run the project, while in the project directory:
```
docker-compose up -d
```

To stop the running containers, while in the project directory:
```
docker-compose down
```

## Data
MySql database files, and project code are referenced as external volumes and will not get lost
during start/stopping the server.

## Useful Commands
    
```
# List all running containers
docker ps -a
```

```
# Inspect all details about a given container.
docker ps -a
```

```
# Access bash shell into a given container.
docker exec -i -t <ID> /bin/bash
```

For more information, please refer to Docker official.

Happy codding.