# Cloud Infrastructure Components

## Introduction

Cloud infrastructure is made up of several components that work together to provide computing services. In this laboratory, the Linux environment provided by the KillerCoda Playground was investigated to identify compute, storage, networking, and operating system resources.

Understanding these components is important because they form the foundation of cloud computing infrastructure.

## 1. Compute Resources

### Purpose

Compute resources provide the processing power needed to execute applications, commands, and workloads. The CPU is one of the main compute resources of a computer system because it processes instructions and performs calculations.

### Importance in Cloud Computing

Compute resources are essential in cloud computing because applications and services need processing power to operate. Cloud providers allow organizations to obtain computing resources without having to purchase and maintain physical servers themselves.

Cloud computing platforms can provide virtual machines and other computing resources that can be increased or decreased depending on the requirements of a workload.

### Relation to the KillerCoda Linux Environment

The KillerCoda environment provides a Linux server with CPU resources that can be investigated using Linux commands. The `lscpu` command can be used to view information about the CPU, while `nproc` can be used to determine the number of available processing units.

Example commands:

```bash
lscpu
nproc
```

The CPU information obtained from these commands represents the compute resources available in the Linux environment.

---

## 2. Storage Resources

### Purpose

Storage resources are used to store operating system files, applications, configurations, and other data. Storage allows information to remain available so that it can be accessed when needed.

### Importance in Cloud Computing

Storage is an important component of cloud computing because applications and users need a reliable place to store data. Cloud providers offer different types of storage for different purposes, such as storing files, application data, backups, and other information.

Cloud storage also allows organizations to store data without having to maintain all of the physical storage hardware themselves.

### Relation to the KillerCoda Linux Environment

The KillerCoda Linux environment contains disk storage that can be examined using Linux commands. The `df -h` command displays information about disk usage and mounted file systems, while `lsblk` displays information about available storage devices.

Example commands:

```bash
df -h
lsblk
```

These commands help identify the storage resources available to the Linux server.

---

## 3. Networking Resources

### Purpose

Networking resources allow computers, servers, applications, and users to communicate with one another. Network interfaces and IP addresses are examples of resources that allow a computer to participate in a network.

### Importance in Cloud Computing

Networking is essential in cloud computing because cloud resources need to communicate with users and with other resources. For example, a cloud server may need to communicate with a database, storage service, application, or user through a network.

Cloud providers provide virtual networking services that allow engineers to organize and control communication between cloud resources.

### Relation to the KillerCoda Linux Environment

The KillerCoda Linux server has network interfaces and an IP address that allow it to communicate over a network. The `hostname -I` command can be used to display the IP address, while `ip addr` provides information about the network interfaces.

Example commands:

```bash
hostname -I
ip addr
```

The information obtained from these commands demonstrates how networking resources are present in the Linux cloud environment.

---

## 4. Operating System

### Purpose

An operating system manages computer hardware and provides an environment where applications and commands can run. It acts as an interface between the user, applications, and the underlying hardware.

### Importance in Cloud Computing

Operating systems are important in cloud computing because cloud servers need an operating environment in which applications and services can execute. Linux is commonly used in server and cloud environments because it provides powerful command-line tools and system-management capabilities.

### Relation to the KillerCoda Linux Environment

The KillerCoda Playground provides a Linux environment that can be accessed through the terminal. The operating system can be identified using the following command:

```bash
cat /etc/os-release
```

The Linux environment allows users to investigate the server's hardware, storage, networking, and other system resources through command-line tools.

---

## Relationship Between the Components

Compute, storage, networking, and the operating system work together to form a functioning cloud infrastructure.

The **compute resources** provide processing power for workloads. The **storage resources** provide space for operating system files, applications, and data. The **networking resources** allow the server and other systems to communicate. The **operating system** manages the available hardware resources and provides the environment needed to run applications and commands.

For example, when a user accesses an application hosted on a cloud server, the operating system manages the server, compute resources process the application's workload, storage resources provide the necessary data, and networking resources allow communication between the user and the server.

## Summary

The investigation of the KillerCoda Linux environment demonstrated that cloud infrastructure consists of multiple components that work together. Compute, storage, networking, and the operating system each have different responsibilities, but they depend on one another to provide a functional computing environment.

Understanding these components provides a foundation for learning how larger cloud infrastructures are designed, deployed, and managed.
