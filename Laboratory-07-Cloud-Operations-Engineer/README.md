# Laboratory 7 — The Cloud Operations Engineer

## Mission Overview

This laboratory activity focuses on monitoring a Linux host and a containerized web application using KillerCoda and Docker. The Nginx web server was deployed in a container, test HTTP requests were generated, application logs were inspected, and real-time container resource usage was observed.

## Objectives

- Check the host server's RAM, disk capacity, and CPU activity.
- Deploy an Nginx web server using Docker.
- Generate successful HTTP requests and an HTTP 404 error.
- Inspect application logs to identify request outcomes.
- Monitor container CPU, memory, and network usage.
- Document the results and screenshots in a GitHub portfolio.

## Monitoring Commands Executed

| Command | Purpose |
|---|---|
| `free -h` | Check memory information |
| `df -h /` | Check root filesystem storage |
| `top` | Observe running processes and CPU activity |
| `docker run -d --name client-website -p 8080:80 nginx` | Deploy the Nginx container |
| `docker ps` | Verify the running container |
| `curl http://localhost:8080` | Generate successful HTTP requests |
| `curl http://localhost:8080/hidden-admin-page` | Generate a request for a nonexistent page |
| `docker logs client-website` | Inspect application logs |
| `docker stats` | Monitor real-time container metrics |

## Skills Learned

- Linux system resource monitoring
- Docker container deployment
- HTTP request testing
- Application log analysis
- Real-time container monitoring
- Markdown documentation and GitHub portfolio management

## Screenshots

- [Memory Check](screenshots/Checkpoint%202_memory-check.png)
- [Disk Check](screenshots/Checkpoint%202_disk-check.png)
- [Nginx Deployment](screenshots/Checkpoint%203_install-nginx.png)
- [Successful HTTP Requests](screenshots/Checkpoint%203_simulation1.1.png)
- [HTTP 404 Error](screenshots/Checkpoint%203_simulation2.png)
- [Docker Logs](screenshots/Checkpoint%204_docker-logs.png)
- [Container Metrics](screenshots/Checkpoint%205_container-metrics.png)

## Conclusion

This laboratory activity provided practical experience in checking host resources, deploying a web server, generating HTTP traffic, analyzing container logs, and monitoring resource consumption using Docker.
