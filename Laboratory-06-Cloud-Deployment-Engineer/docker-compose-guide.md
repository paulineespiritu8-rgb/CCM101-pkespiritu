# Docker Compose Guide

## What does the services: block do?

The services: block defines the containers that Docker Compose will create and manage. In this project, it defines the database and app containers.

## How did the Nextcloud app container know how to find the database container?

The Nextcloud container uses the environment variable MYSQL_HOST=database. The value database matches the name of the database service, allowing the application to connect to the database container.

## What is the difference between docker run and docker-compose up -d?

docker run starts a single container using a command. docker-compose up -d starts multiple containers defined in a docker-compose.yml file using a single command.
