### multi-tier-architecture.md

```markdown
# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture separates an application into two main parts: the Web/Application Tier and the Database Tier. In this mission, Nextcloud is used as the Web/Application Tier while MariaDB is used as the Database Tier.

## The Web/Application Tier

The Web/Application Tier is responsible for serving the user interface and handling HTTP requests. In this mission, the Nextcloud container provides the web application that users access through a browser.

## The Database Tier

The Database Tier is responsible for storing persistent data, user accounts, and other information needed by the application. In this mission, the MariaDB container is used as the database for Nextcloud.

## Why Separate Them?

Separating the web application and database into different containers keeps their responsibilities separate. It also makes the system easier to manage because the application and database can be handled independently.
