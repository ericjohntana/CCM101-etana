# Mission 4 Reflection

## Reflection

This laboratory activity gave me a better understanding of how containers work compared to Virtual Machines. A Virtual Machine requires a complete operating system, which can make the startup and installation process take more time. Docker containers are different because they share the host operating system kernel, allowing applications to start faster. I learned that this makes containers useful when applications need to be deployed quickly and with fewer resources.

The port mapping `-p 8080:80` allows me to access the Nginx web server running inside the Docker container. Port 80 is the port used by Nginx inside the container, while port 8080 is used on the host. By connecting these two ports, I was able to use `curl http://localhost:8080` to check if the Nginx server was working properly.

I also learned what happens when a container is removed using the `docker rm` command. The container is permanently removed after it has been stopped. Data that was stored only inside the container may also be lost if it was not stored using a persistent storage method. This helped me understand the importance of using proper storage when working with applications that need to keep data.

Containerization can improve collaboration between developers and IT operations teams. Developers can create an application together with its required dependencies, while IT operations teams can use the same container when deploying the application. This can help make the development and deployment process more consistent.

My GitHub portfolio is also improving as I add more laboratory activities and technical documentation. Through this activity, I gained practical experience with Docker, Nginx, containers, and GitHub. It also helped me become more familiar with documenting my work and organizing my cloud computing projects.
