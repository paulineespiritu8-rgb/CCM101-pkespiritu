# Firewall Configuration

## 1. Allow SSH

Command:

sudo ufw allow ssh

This command allows SSH connections so administrators can manage the server remotely.

## 2. Set the Default Deny Policy

Commands:

sudo ufw default deny incoming
sudo ufw default allow outgoing
The first command blocks incoming traffic by default, while the second allows outgoing traffic.

## 3. Allow Port 8080

Command:

sudo ufw allow 8080/tcp

This command allows incoming TCP traffic on port 8080 for the web application.

## 4. What Happens if UFW Is Enabled Before Allowing SSH?
If sudo ufw enable is run before sudo ufw allow ssh, SSH access may be blocked, preventing remote administrators from connecting to the server.
