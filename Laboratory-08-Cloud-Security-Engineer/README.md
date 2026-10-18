# Laboratory 08: The Cloud Security Engineer

## Mission Overview

This mission focuses on securing an Ubuntu server using the Uncomplicated Firewall (UFW). The activity includes deploying an Nginx web application, checking network access, and configuring firewall rules to allow SSH and port 8080 while blocking other incoming traffic by default.

## Objectives

- Understand the Principle of Least Privilege.
- Identify the attack surface of a virtual machine.
- Perform a basic network port security audit.
- Configure UFW with a Default Deny policy.
- Allow SSH and TCP traffic on port 8080.
- Document security configurations using Markdown.

## Commands Executed

```bash
docker run -d --name secure-web-app -p 8080:80 nginx
curl http://localhost:8080
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered

## Skills Learned
- Deploying an Nginx web server using Docker.
- Testing web application connectivity with curl.
- Configuring firewall rules in Ubuntu.
- Applying the Default Deny security policy.
- Managing network ports and SSH access.
- Writing technical documentation in Markdown.
- Organizing a cloud computing portfolio on GitHub.
