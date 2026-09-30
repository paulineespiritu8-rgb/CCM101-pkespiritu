# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block defines the containers that Docker Compose will create and manage. In this project, it defines the `database` and `app` services. The database uses MariaDB, while the app uses Nextcloud.

## How Did the Nextcloud App Container Know How to Find the Database Container?

The Nextcloud container uses `MYSQL_HOST=database`. The value `database` matches the database service name, allowing Nextcloud to connect to MariaDB through the Docker network.

## What Is the Difference Between `docker run` and `docker-compose up -d`?

The `docker run` command starts an individual container. Meanwhile, `docker-compose up -d` starts the services defined in the `docker-compose.yml` file with one command. The `-d` option runs the containers in the background.
