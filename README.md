# Collection of Docker Compose containers

This is a quickstart repository which contains several useful docker-compose scripts.

## Pre-Requisites

Docker 18.06 or greater

## Getting Started

Clone this repository

    git clone git@github.com:brucem91/Docker-Containers.git

CD into directory

    cd Docker-Containers

Each service follows the same pattern. To start MySQL (for example)

    cd mysql
    docker-compose up -d

And to powerdown a service:

    docker-compose down

Or to completely remove the service:

    docker-compose down --remove-orphans

## Configuring your Container

If you need to make any changes to a container, you may create a docker-compose.override.yml
file. As applicable, an example docker-compose.override.yml.example will be provided as
reference.

Typically you may want to use the override file to customize the port or default password
that a container may use. You should generally be able to override any setting that it on the
base docker-compose.yml file.

For additional reference, please consult the given container's documentation as well as the
docker-compose documentation.

## Common Commands

Display all running containers

    docker ps -a

View log for a given container (where abc is the first few characters to identify the container)

    docker logs abc

How to stop a container

    docker stop abc

How to remove a container

    docker rm abc
    
Display all images

    docker images

