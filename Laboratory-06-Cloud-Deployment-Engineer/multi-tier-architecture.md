# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is a system design that separates an application into two main parts: the Web/Application Tier and the Database Tier. These tiers work together to provide services to users while keeping application processing and data storage separate.

## The Web/Application Tier

The Web/Application Tier handles the application's interface and user requests. In this laboratory activity, Nextcloud serves as the web application that users access through a browser. It communicates with the database to retrieve and store the information required by the application.

## The Database Tier

The Database Tier stores and manages the application's data. In this deployment, MariaDB serves as the database for Nextcloud. It stores information such as user accounts and file metadata needed by the application.

## Why Separate Them?

Separating the web application and database into two containers makes the system easier to manage, maintain, and troubleshoot. Each container has its own responsibility, and either service can be updated or managed independently without combining both components into one container.

## Architecture Used in This Laboratory

- **Application:** Nextcloud
- **Database:** MariaDB 10.6
- **Container Management:** Docker Compose
- **Web Access:** Port 8080
- **Database Connection:** The `MYSQL_HOST=database` environment variable

Nextcloud communicates with MariaDB through the internal Docker Compose network using the database service name `database`.
