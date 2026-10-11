## Mission Overview

This mission focuses on monitoring a Linux server and a containerized web application as a Cloud Operations Engineer at CloudNova Technologies, preparing the infrastructure for high user traffic from an upcoming client campaign. Using the KillerCoda Playground and Docker, tasks include establishing a clear baseline of the host’s CPU, memory, and disk capacity, deploying an Nginx web server, generating both normal and error test traffic, retrieving and analyzing application logs to verify request statuses, and examining real-time container metrics to confirm efficient resource consumption. All results and evidence are properly documented in Markdown and stored in the GitHub Cloud Computing Portfolio.


## Objectives

- Monitor host CPU, memory, and disk capacity.
- Deploy an Nginx web server using Docker.
- Generate HTTP requests and identify a 404 error.
- Retrieve and analyze application logs.
- Monitor container CPU, memory, and network usage.
- Document the results using Markdown and GitHub.

## Monitoring Commands Executed

| Command | Purpose |
|---|---|
| free -h | Check memory usage and available RAM. |
| df -h / | Check root filesystem disk capacity. |
| top | Monitor CPU usage and running processes. |
| docker run -d --name client-website -p 8080:80 nginx | Deploy the Nginx container. |
| curl -i http://localhost:8080/ | Send an HTTP request to the website. |
| curl -i http://localhost:8080/hidden-admin-page | Test a nonexistent page. |
| docker logs client-website | Retrieve application logs. |
| docker stats client-website | Monitor container resource usage. |

## Skills Learned

- Linux system monitoring
- Docker container deployment
- HTTP traffic simulation
- Application log analysis
- Container performance monitoring
- Markdown documentation
- GitHub repository management
