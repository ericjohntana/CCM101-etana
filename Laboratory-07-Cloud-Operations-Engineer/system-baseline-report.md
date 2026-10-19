# System Baseline Report

## Overview

This report records the initial system health of the KillerCoda server before deploying the client website.

## Memory Check

Command executed:

```bash
free -h
```

- **Total RAM:** 1.9 GiB

## Disk Check

Command executed:

```bash
df -h /
```

- **Root Filesystem Total Capacity:** 19G

## CPU and Process Monitoring

Command executed:

```bash
top
```

The running processes and CPU activity were observed using the terminal task monitor.

## Importance of Disk Monitoring

Checking disk space before a massive traffic surge is important because insufficient storage can prevent the server from writing logs, temporary files, and application data, potentially affecting website performance and availability.
