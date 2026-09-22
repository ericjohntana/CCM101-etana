# Laboratory 04 – The Cloud-Native Engineer

## Mission Overview

This laboratory activity introduces cloud-native engineering and containerization using Docker. The activity focuses on understanding the differences between traditional Virtual Machines (VMs) and Containers and demonstrates how Docker can be used to deploy and manage a containerized web server.

Using the KillerCoda Docker environment, an Nginx web server was deployed inside a Docker container. The activity also covered basic Docker commands for checking the Docker environment, running containers, stopping containers, and removing containers.

## Objectives

The objectives of this laboratory activity are:

* Differentiate between Virtual Machines and Containers.
* Access a Docker-enabled cloud environment using KillerCoda.
* Execute fundamental Docker CLI commands.
* Pull and run an Nginx container.
* Manage the lifecycle of a Docker container.
* Document container operations using Markdown.
* Maintain an organized GitHub Cloud Computing Portfolio.

## Docker Commands Executed

### Check Docker Version

```bash
docker --version
```

### Check Docker Status

```bash
docker info
```

### Pull the Nginx Image

```bash
docker pull nginx
```

### Run the Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

### Test the Nginx Web Server

```bash
curl http://localhost:8080
```

### List Running Containers

```bash
docker ps
```

### Stop the Nginx Container

```bash
docker stop nginx-server
```

### Verify the Container Is Stopped

```bash
docker ps
```

### Remove the Container

```bash
docker rm nginx-server
```

## Skills Learned

Through this laboratory activity, I learned how to:

* Understand the basic concept of containerization.
* Compare Virtual Machines and Containers.
* Use the Docker command-line interface.
* Download Docker images from Docker Hub.
* Run an Nginx web server inside a container.
* Map a host port to a container port.
* Check running Docker containers.
* Stop and remove Docker containers.
* Document technical procedures using Markdown.
* Organize and maintain a GitHub portfolio.

## Challenges Encountered

One challenge encountered during this activity was becoming familiar with Docker commands and understanding how containers work. Another challenge was making sure that the correct port mapping was used so that the Nginx web server could be accessed through port 8080.

The activity also required careful documentation of each command and its output. Taking screenshots after completing the required commands helped provide evidence that the Docker operations were successfully performed.

