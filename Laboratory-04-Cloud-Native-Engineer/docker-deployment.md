# Docker Deployment

## Docker Environment

The Docker environment was accessed through the KillerCoda Playground.

### 1. Check Docker Version

```bash
docker --version
```

This command displays the installed Docker version.

### 2. Check Docker Environment Status

```bash
docker info
```

This command displays detailed information about the Docker installation and Docker environment.

## Nginx Deployment

### 3. Pull the Nginx Image

```bash
docker pull nginx
```

This command downloads the official Nginx image from Docker Hub.

### 4. Run the Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

This command creates and starts an Nginx container in detached mode while mapping host port 8080 to container port 80.

### 5. Test the Nginx Web Server

```bash
curl http://localhost:8080
```

This command sends an HTTP request to the Nginx server and verifies that the web server is responding.

## Container Lifecycle

### 6. List Running Containers

```bash
docker ps
```

This command displays the Docker containers that are currently running.

### 7. Stop the Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container.

### 8. Verify the Container Is Stopped

```bash
docker ps
```

This command verifies that the Nginx container is no longer running.

### 9. Remove the Container

```bash
docker rm nginx-server
```

This command removes the stopped Nginx container from the Docker environment.

## Summary

The Docker lifecycle demonstrated in this activity included pulling an image, creating and running a container, testing the application, stopping the container, verifying its status, and finally removing it.
