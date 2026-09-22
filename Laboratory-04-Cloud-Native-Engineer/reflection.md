# Mission 4 Reflection

## Reflection

This laboratory activity helped me understand the difference between using a traditional Virtual Machine and using Docker containers. A Virtual Machine needs to start a complete operating system before applications can run, so the boot and setup process can take more time. In comparison, a Docker container uses the host operating system kernel and can start much faster. Because of this, containers can make application deployment more lightweight and efficient.

The port mapping `-p 8080:80` is necessary because the Nginx web server is running inside the container on port 80, while port 8080 is exposed on the host. The mapping connects the host port to the container port, allowing me to send a request to `http://localhost:8080` and access the Nginx web server. Without the port mapping, the service inside the container would not be directly accessible through the host's port 8080.

When the `docker rm` command is used, the Docker container itself is removed. Any data stored only inside the container that is not saved using a persistent storage method can be lost when the container is removed. This shows why applications that need persistent data should use appropriate storage solutions such as volumes.

Containerization can also change how developers and IT operations teams work together. Developers can package an application with its dependencies, while operations teams can deploy the same containerized application in different environments. This supports a more consistent workflow between development and operations.

My GitHub portfolio is evolving by adding practical cloud computing activities and technical documentation. This laboratory added Docker and containerization experience to my portfolio and helped me practice using GitHub to organize and document my work.
