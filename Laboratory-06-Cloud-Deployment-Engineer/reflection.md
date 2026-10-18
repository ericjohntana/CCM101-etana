# Reflection — The Cloud Deployment Engineer

In this laboratory activity, I learned how Docker Compose makes deploying an application easier. Instead of typing separate commands to set up each container, I used a `docker-compose.yml` file to configure Nextcloud and MariaDB. With one command, I was able to start both services together. This made the deployment more organized and easier to manage.

I also learned that YAML indentation is important when creating a configuration file. If I use the wrong indentation or a Tab instead of spaces, the file may not work correctly because YAML follows a specific structure. I also understood the purpose of environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_HOST`. These settings provide the database credentials and connection information that Nextcloud needs to communicate with MariaDB.

Deploying Nextcloud was a good experience because I was able to run a private cloud storage application and access its installation page through a web browser. Seeing the application work after entering commands in the terminal helped me understand how Docker containers work together. I also learned how to check the status of the containers and shut down the deployment properly using Docker Compose.

Since Mission 1, my understanding of cloud computing has improved. I have become more familiar with cloud technologies, Linux commands, Docker, and managing applications. Before, I mainly learned about basic cloud concepts, but now I understand how different services can work together to provide an application. Overall, this activity helped me improve my technical skills and understand why configuration files are useful in deploying and managing cloud infrastructure.
