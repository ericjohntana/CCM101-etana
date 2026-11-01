# Mission 8 – Reflection

Completing this laboratory activity helped me understand the importance of securing a cloud server using a host-based firewall. A host-based firewall provides an additional layer of protection even if the physical network perimeter is breached. It controls incoming and outgoing network traffic directly on the server and blocks connections that are not permitted by the configured rules.

Managing open network ports is also important because every unnecessary open port can become a possible entry point for attackers. By allowing only the ports required by the application, administrators can reduce the server's attack surface and minimize security risks. In this activity, I learned how to use UFW to allow SSH for remote administration and port 8080 for the Nginx web application while blocking other incoming connections by default.

In a real enterprise environment, leaving a database port such as 3306 for MySQL open to the public internet is dangerous. Attackers could attempt unauthorized access, brute-force attacks, or exploit database vulnerabilities. Database services should only be accessible to trusted applications and authorized administrators.

This mission also changed my perspective on how easily a server can become vulnerable when security is not properly configured. Before this activity, I did not fully understand the importance of firewall rules and network port management. I learned that even a working web application needs proper security configurations to protect its services and data.

Completing eight cloud computing missions has helped me improve my knowledge of Linux, Docker, cloud infrastructure, server management, and security. My GitHub portfolio now contains different laboratory activities that demonstrate my learning progress and practical skills. I am more confident in performing basic cloud administration tasks and documenting my work professionally. This experience also taught me that server security is not a one-time task but a continuous responsibility.
