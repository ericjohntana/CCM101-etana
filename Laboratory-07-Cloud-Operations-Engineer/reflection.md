# Mission 7 — Reflection

This laboratory activity helped me understand the importance of monitoring a server before and after deploying a web application. Using Linux commands such as `free -h`, `df -h /`, and `top`, I learned how to check the server's memory, disk capacity, and running processes. Even if containers are running properly, the host server still needs enough resources to support them. Limited memory or disk space can affect application performance and may cause services to fail, especially when many users access the website at the same time.

I also learned how the `docker logs` command helps troubleshoot application problems. When a user cannot access a website or log in to an application, the logs can provide useful information about requests, errors, and application activity. In this laboratory, I generated successful HTTP requests and intentionally requested a nonexistent page to produce a 404 error. Examining the logs helped me identify the failed request and understand how logs support troubleshooting.

Another important lesson was the difference between logs and metrics. Logs record events and provide details about what happened, while metrics show numerical measurements such as CPU usage, memory consumption, and network activity. Using `docker stats`, I was able to observe the container's resource usage in real time. Both logs and metrics are important because they provide different information needed to investigate and prevent problems.

For large enterprise environments, monitoring thousands of containers manually would be difficult. Tools such as Prometheus can collect and store metrics, while Grafana can display them through dashboards and visualizations. These tools help engineers monitor infrastructure and identify unusual behavior.

This activity improved my confidence in using Linux and Docker commands. I learned to check system resources, generate test traffic, inspect logs, and observe container metrics. These skills are useful for maintaining reliable applications and troubleshooting cloud infrastructure.
