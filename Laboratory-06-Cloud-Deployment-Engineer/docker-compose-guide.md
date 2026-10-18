# Docker Compose Guide

## Overview

In this activity, I used Docker Compose to run Nextcloud and MariaDB together. I created a `docker-compose.yml` file to put the settings of both services in one place.

## The `services:` Block

The `services:` block contains the two services used in this activity:

- **database:** Uses MariaDB to store the data needed by Nextcloud.
- **app:** Uses Nextcloud to provide the website that users can open through a browser using port 8080.

## Database Connection

Nextcloud needs a database to work properly. The `MYSQL_HOST=database` setting tells Nextcloud where to find MariaDB. The word `database` matches the database service name in the Compose file.

The other settings, such as `MYSQL_DATABASE`, `MYSQL_USER`, and `MYSQL_PASSWORD`, provide the database name, username, and password used for the connection.

## Docker Run vs. Docker Compose

The `docker run` command is usually used to start one container at a time. Docker Compose allows me to manage multiple related services using one configuration file.

In this activity, I used `docker-compose up -d` to start Nextcloud and MariaDB. I used `docker-compose ps` to check if both services were running and `docker-compose down` to stop and remove the containers.

## Infrastructure as Code (IaC)

Infrastructure as Code means using a configuration file to describe how an application should be set up. In this activity, the `docker-compose.yml` file contained the settings needed to run Nextcloud and MariaDB.

## Conclusion

Through this activity, I learned how to use Docker Compose to run two services together. I also learned how Nextcloud connects to MariaDB and how to start, check, and stop the containers using terminal commands.
