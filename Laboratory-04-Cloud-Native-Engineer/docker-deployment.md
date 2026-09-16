## Docker Environment

| Command | Explanation |
|---|---|
| docker --version | Checks the installed Docker version. |
| docker info | Displays information about the current Docker environment. |


## Checkpoint 4: Nginx Deployment

| Command | Explanation |
|---|---|
| docker pull nginx | Pulls the official Nginx image. |
| docker run -d -p 8080:80 --name nginx-server nginx | Runs Nginx in detached mode and maps port 8080 to port 80. |
| curl http://localhost:8080 | Checks if the Nginx web server is running. |


## Checkpoint 5: Container Lifecycle

| Command | Explanation |
|---|---|
| docker ps | Lists the running containers. |
| docker stop nginx-server | Stops the Nginx container. |
| docker ps | Verifies that the container has stopped. |
| docker rm nginx-server | Removes the stopped container. |

