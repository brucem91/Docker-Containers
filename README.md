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