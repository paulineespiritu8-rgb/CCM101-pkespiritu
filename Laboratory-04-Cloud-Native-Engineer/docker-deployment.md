## Docker Environment

| Command | Explanation |
|---|---|
| docker --version | Checks the installed Docker version. |
| docker info | Displays information about the current Docker environment. |

| Screenshot | Filename |
|---|---|
| Docker verification | docker-version.png |

## Checkpoint 4: Nginx Deployment

| Step | Command | Explanation |
|---|---|---|
| 1 | docker pull nginx | Pulls the official Nginx image. |
| 2 | docker run -d -p 8080:80 --name nginx-server nginx | Runs Nginx in detached mode and maps port 8080 to port 80. |
| 3 | curl http://localhost:8080 | Checks if the Nginx web server is running. |

| Verification | Expected Result |
|---|---|
| curl http://localhost:8080 | Nginx welcome page containing *“Welcome to nginx!”* |

| Screenshot | Filename |
|---|---|
| Nginx verification | nginx-running.png |

## Checkpoint 5: Container Lifecycle

| Step | Command | Explanation |
|---|---|---|
| 1 | docker ps | Lists the running containers. |
| 2 | docker stop nginx-server | Stops the Nginx container. |
| 3 | docker ps | Verifies that the container has stopped. |
| 4 | docker rm nginx-server | Removes the stopped container. |

| Screenshot | Filename |
|---|---|
| Container lifecycle | container-lifecycle.png |
