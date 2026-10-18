# Laboratory 6 — The Cloud Deployment Engineer

## Mission Overview

This laboratory activity focuses on deploying Nextcloud and MariaDB using Docker Compose. Both services are configured in one `docker-compose.yml` file and run together as a private cloud storage application.

## Objectives

- Understand two-tier application architecture.
- Create a Docker Compose configuration file using nano.
- Deploy Nextcloud and MariaDB using Docker Compose.
- Access Nextcloud through a web browser.
- Check the containers and shut down the deployment.
- Document the activity using Markdown and screenshots.

## Technologies Used

- KillerCoda Ubuntu/Docker Playground
- Docker
- Docker Compose
- Nextcloud
- MariaDB 10.6
- YAML
- Markdown
- GitHub

## Commands Executed

### 1. Create the Project Directory

```bash
mkdir nextcloud-deployment
```

Creates a folder named `nextcloud-deployment` for the project files.

```bash
cd nextcloud-deployment
```

Moves into the project directory.

### 2. Create the Configuration File

```bash
nano docker-compose.yml
```

Opens the nano text editor to create and edit the Docker Compose configuration file.

### 3. Display the Configuration

```bash
cat docker-compose.yml
```

Displays the contents of the configuration file in the terminal.

### 4. Deploy the Services

```bash
docker-compose up -d
```

Starts the Nextcloud and MariaDB services in the background using the configuration file.

### 5. Check the Containers

```bash
docker-compose ps
```

Shows the status of the containers and their port information.

### 6. Shut Down the Deployment

```bash
docker-compose down
```

Stops and removes the containers and the Docker Compose network created for the deployment.

## Skills Learned

- Understanding two-tier application architecture.
- Creating YAML configuration files.
- Using Docker Compose to manage multiple containers.
- Connecting Nextcloud to a MariaDB database.
- Accessing a containerized application through a browser.
- Checking container status and shutting down a deployment.
- Documenting laboratory activities using GitHub and Markdown.

## Screenshots (Required)

The `screenshots/` folder contains the evidence collected during the activity:

## Screenshots

- [compose-deployment.png](screenshots/Checkpoint%204-compose-deployment.png) — Shows the running containers.
- [nextcloud-web.png](screenshots/Checkpoint%205-nextcloud-web.png) — Shows the Nextcloud installation page.
- [compose-teardown.png](screenshots/Checkpoint%205-compose-teardown.png) — Shows the containers being stopped and removed.

## Conclusion

Through this activity, I learned how to deploy and manage Nextcloud and MariaDB using Docker Compose. I also gained experience with terminal commands, YAML configuration, and documenting the deployment process.

