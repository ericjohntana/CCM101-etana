# Laboratory 8 – The Cloud Security Engineer

## Mission Overview

This laboratory activity focuses on securing an Ubuntu server using UFW (Uncomplicated Firewall). The activity involves deploying an Nginx web application using Docker, auditing network access, and configuring firewall rules to protect the server from unauthorized incoming connections.

## Objectives

- Understand the Principle of Least Privilege.
- Identify the attack surface of a virtual machine.
- Understand the Default Deny firewall policy.
- Deploy an Nginx web application using Docker.
- Configure and activate UFW.
- Allow SSH and TCP port 8080.
- Document firewall configurations using Markdown.

## Commands Executed

### 1. Deploy Nginx

```bash
docker run -d --name secure-web-app -p 8080:80 nginx
```

Creates and runs an Nginx container named `secure-web-app` in the background and maps port 8080 to port 80.

### 2. Test the Web Application

```bash
curl http://localhost:8080
```

Sends a request to the Nginx web application to check if it is working correctly.

### 3. Allow SSH

```bash
sudo ufw allow ssh
```

Allows SSH connections through port 22 so administrators can remotely access the server.

### 4. Configure Default Firewall Policies

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

Blocks incoming connections by default while allowing outgoing network traffic.

### 5. Enable Firewall

```bash
sudo ufw enable
```

Activates UFW and applies the configured firewall rules.

### 6. Check Firewall Status

```bash
sudo ufw status verbose
```

Displays the firewall status, default policies, and configured rules.

### 7. Allow Port 8080

```bash
sudo ufw allow 8080/tcp
```

Allows incoming TCP connections through port 8080 for the Nginx web application.

### 8. Verify Firewall Rules

```bash
sudo ufw status numbered
```

Displays the firewall rules with numbers to verify the allowed ports and connections.

## Skills Learned

- Linux server security.
- Docker container deployment.
- Network port management.
- UFW firewall configuration.
- Applying the Default Deny security policy.
- Understanding cloud security principles.
- Technical documentation using Markdown.
- GitHub portfolio management.

## Screenshots

| Screenshot | Description |
|---|---|
| [vulnerable-app-running.png](screenshots/Checkpoint20%320%-20%vulnerable-app-running.png) | Shows the running Nginx application. |
| [firewall-activated.png](screenshots/Checkpoint20%420%-20%firewall-activated.png) | Shows the active UFW firewall. |
| [firewall-port-allowed.png](screenshots/Checkpoint20%520%-20%firewall-port-allowed.png) | Shows the allowed firewall ports and successful Nginx response. |

This laboratory activity provided practical experience in securing a cloud server using UFW. It demonstrated the importance of controlling incoming network traffic, allowing only necessary services, and reducing the attack surface of a server.
