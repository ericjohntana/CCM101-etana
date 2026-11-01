# Firewall Configuration

## Overview

This document contains the commands used to secure the Ubuntu server using UFW (Uncomplicated Firewall). The firewall was configured to block incoming traffic by default while allowing SSH connections and the Nginx web application through port 8080.

## 1. Allow SSH

```bash
sudo ufw allow ssh
```

This command allows SSH connections through port 22 so administrators can remotely manage the server.

**Terminal Output:**

```text
Rules updated
Rules updated (v6)
```

## 2. Configure Default Firewall Policies

**Block incoming traffic by default:**

```bash
sudo ufw default deny incoming
```

**Allow outgoing traffic by default:**

```bash
sudo ufw default allow outgoing
```

These commands block incoming connections unless explicitly allowed while permitting outgoing connections.

## 3. Enable the Firewall

```bash
sudo ufw enable
```

This command activates the firewall and applies the configured security rules.

## 4. Verify Firewall Status

```bash
sudo ufw status verbose
```

The firewall status showed:

```text
Status: active
Logging: on (low)
Default: deny (incoming), allow (outgoing), deny (routed)
```

SSH was successfully allowed through port 22.

## 5. Allow Port 8080

```bash
sudo ufw allow 8080/tcp
```

This command allows incoming TCP connections through port 8080 so users can access the Nginx web application.

## 6. Verify Firewall Rules

```bash
sudo ufw status numbered
```

The firewall displayed the following allowed ports:

- Port 22 – SSH
- Port 8080 – Nginx web application

Both IPv4 and IPv6 rules were successfully added.

## 7. Test the Web Application

```bash
curl http://localhost:8080
```

The command returned the Nginx welcome page, confirming that the web application was responding successfully.

## 8. SSH Security Reminder

If `sudo ufw enable` is executed before `sudo ufw allow ssh`, incoming SSH connections may be blocked, potentially causing administrators to lose remote access to the server.

The UFW firewall was successfully activated with a Default Deny incoming policy and an Allow outgoing policy. SSH and TCP port 8080 were explicitly permitted to support remote administration and web application access.
