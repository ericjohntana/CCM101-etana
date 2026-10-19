# Container Observability Report

## Application Logs

Command executed:

```bash
docker logs client-website
```

The container logs were checked to identify successful HTTP requests and a failed request.

### Successful HTTP Requests

The logs showed three successful requests with HTTP status code `200`.

```text
172.17.0.1 - - [19/Oct/2026:15:25:07 +0000] "GET / HTTP/1.1" 200 896 "-" "curl/8.5.0" "-"
172.17.0.1 - - [19/Oct/2026:15:25:31 +0000] "GET / HTTP/1.1" 200 896 "-" "curl/8.5.0" "-"
172.17.0.1 - - [19/Oct/2026:15:25:48 +0000] "GET / HTTP/1.1" 200 896 "-" "curl/8.5.0" "-"
```

### HTTP 404 Error Log

The following log entry shows the request to a nonexistent page.

```text
172.17.0.1 - - [19/Oct/2026:15:29:57 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
```

### Importance of Application Logs

Application logs are vital for troubleshooting because they record HTTP requests and errors that help identify what happened when a problem occurred. They allow engineers to investigate failed requests and determine the next steps toward resolving an issue.

![Docker Logs](screenshots/Checkpoint%204_docker-log.png)

## Real-Time Container Metrics

Command executed:

```bash
docker stats
```

The following metrics were recorded for the `client-website` container.

| Metric | Recorded Value |
|---|---|
| Container Name | `client-website` |
| CPU Usage | 0.00% |
| Memory Usage | 2.766MiB |
| Memory Limit | 1.859GiB |
| Memory Percentage | 0.15% |
| Network I/O | 3.95kB / 5.33kB |
| Block I/O | 49.2kB / 12.3kB |
| PIDs | 2 |

![Container Metrics](screenshots/Checkpoint%205_container-metrics.png)

## Summary

The Nginx container's logs showed three successful HTTP requests and one failed request with status code `404`. Docker's real-time statistics showed that the container was using 2.766MiB of memory and 0.00% CPU at the time of observation. These results demonstrate how application logs and container metrics can be used to monitor a web server and investigate errors.
