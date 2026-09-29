# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

In this mission, I deployed a private cloud storage system using Nextcloud and MariaDB. The two containers were connected using Docker Compose to create a two-tier application.

## Objectives

- Explain the concept of a multi-tier application architecture.
- Understand the purpose and structure of a docker-compose.yml file.
- Use a Linux command-line text editor (nano) to create configuration files.
- Deploy a multi-container application (Nextcloud + Database) using Docker Compose.
- Document deployment procedures and Infrastructure as Code (IaC) principles using Markdown.
- Continue expanding the professional GitHub Cloud Computing Portfolio.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```
## Skills Learned

- Understanding two-tier architecture
- Creating a Docker Compose configuration file
- Using the Linux nano text editor
- Deploying multiple containers using Docker Compose
- Using environment variables in Docker Compose
- Accessing a web application through port 8080
- Understanding basic Infrastructure as Code (IaC)
- Documenting cloud deployment using Markdown
