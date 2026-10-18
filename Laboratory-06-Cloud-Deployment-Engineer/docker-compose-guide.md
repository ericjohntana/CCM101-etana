# Docker Compose Guide

## Overview

In this activity, I used Docker Compose to run Nextcloud and MariaDB together using a file named `docker-compose.yml`.

## The `services:` Block

The `services:` block defines the containers used in the application. In my YAML file, there are two services: `database` and `app`. The `database` service uses MariaDB to store data, while the `app` service uses Nextcloud to provide the web interface.

## Database Connection

The Nextcloud container finds the MariaDB container through the `MYSQL_HOST=database` environment variable. The word `database` matches the name of the database service in the YAML file. This allows Nextcloud to connect to MariaDB through the Docker Compose network.

## Docker Run vs. Docker Compose

The `docker run` command is used to create and start an individual container. In contrast, `docker-compose up -d` starts the services defined in the `docker-compose.yml` file together in the background.

In this activity, Docker Compose allowed me to start Nextcloud and MariaDB using one command. I also used `docker-compose ps` to check the containers and `docker-compose down` to stop and remove them.

## Conclusion

Through this activity, I learned how Docker Compose manages multiple containers and how Nextcloud connects to its database. I also learned how to deploy, check, and stop the application using terminal commands.
