# Two-Tier Architecture

A Two-Tier Architecture is a system design that separates an application into two layers: the Web/Application Tier and the Database Tier. These tiers work together to provide services to users.

## The Web/Application Tier

The Web/Application Tier is responsible for serving the user interface and handling HTTP requests. In this project, the Nextcloud container provides the web interface that users access through a browser.

## The Database Tier

The Database Tier is responsible for storing persistent data and user account information. In this project, the MariaDB container stores the data required by the Nextcloud application.

## Why Separate Them?

Keeping the web server and database in separate containers makes the system easier to manage and maintain. If one container needs to be updated or restarted, it can be done without affecting the other container. This setup also improves flexibility and scalability.
