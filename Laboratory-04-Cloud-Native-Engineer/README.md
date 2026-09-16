## Mission Overview

This laboratory activity focuses on containerization and the use of Docker to deploy and manage an Nginx web server. It also explores the differences between Virtual Machines and containers.

## Objectives

- Differentiate Virtual Machines and containers.
- Access a Docker-enabled KillerCoda Playground.
- Execute basic Docker CLI commands.
- Pull, run, manage, and terminate an Nginx container.
- Create technical documentation using Markdown.
- Maintain a GitHub Cloud Computing Portfolio.

## Docker Commands Executed

| Command | Purpose |
|---|---|
| docker --version | Checks the Docker version. |
| docker info | Displays Docker environment information. |
| docker pull nginx | Downloads the official Nginx image. |
| docker run -d -p 8080:80 --name nginx-server nginx | Runs Nginx in the background with port mapping. |
| curl http://localhost:8080 | Verifies the Nginx web server. |
| docker ps | Lists running containers. |
| docker stop nginx-server | Stops the Nginx container. |
| docker rm nginx-server | Removes the container. |

## Skills Learned

I learned how to use Docker commands for downloading images, running containers, checking container status, and managing a containerized web server. I also learned how port mapping allows an Nginx container to be accessed from the host.

## Challenges Encountered

One challenge was becoming familiar with the different Docker commands and their purposes. I also needed to understand how port mapping works when testing the Nginx server through port 8080.
