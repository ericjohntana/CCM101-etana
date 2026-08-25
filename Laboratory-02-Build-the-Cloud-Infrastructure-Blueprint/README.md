# Laboratory 02 – Build the Cloud Infrastructure Blueprint

## Mission Overview

This laboratory focused on investigating the infrastructure that supports cloud computing. The activity involved examining a Linux server using the KillerCoda Playground, identifying cloud infrastructure components, researching major cloud providers, designing a simple cloud infrastructure, and documenting the results using Markdown.

Through this laboratory, I learned how compute, storage, networking, and operating system resources work together to support cloud-based systems. I also practiced using Linux commands to inspect a cloud server and organized my findings as technical documentation in my GitHub Cloud Computing Portfolio.

## Objectives

The objectives of this laboratory were to:

* Explain the major components of cloud infrastructure.
* Investigate hardware and software resources in a Linux environment.
* Differentiate compute, storage, networking, and identity resources.
* Understand the relationship between cloud infrastructure components.
* Create professional technical documentation using Markdown.
* Continue developing the GitHub Cloud Computing Portfolio.

## Cloud Infrastructure Components

The major infrastructure components investigated were:

* Compute
* Storage
* Networking
* Operating System
* Identity and Access Management

### Compute

Compute resources provide the processing power needed to run applications, commands, and services. In a cloud environment, compute resources can be provided through virtual machines or other computing services. During this laboratory, the CPU model and number of CPU cores were investigated using Linux commands.

### Storage

Storage resources are used to store operating system files, applications, configurations, and other data. Storage is an important part of cloud infrastructure because applications need a reliable place to save and access information. In the Linux environment, storage capacity and mounted file systems were investigated using commands such as `df -h` and `lsblk`.

### Networking

Networking resources allow computers, servers, applications, and users to communicate with each other. In cloud computing, networking makes it possible for cloud resources to communicate with users and other services. During this laboratory, the hostname, IP address, and network interfaces of the Linux environment were investigated.

### Operating System

The operating system manages the computer's hardware resources and provides an environment for applications and commands to run. The Linux operating system used in the KillerCoda environment allowed me to interact with the cloud server through the terminal and investigate its resources.

### Identity and Access Management

Identity and Access Management (IAM) is used to manage users, identities, permissions, and access to cloud resources. IAM is important because it helps control who can access resources and what actions they are allowed to perform. Although the Linux investigation mainly focused on compute, storage, networking, and the operating system, IAM was included as an important infrastructure component when comparing major cloud providers.

## Tools Used

The following tools were used during this laboratory:

* KillerCoda Playground
* Linux terminal
* GitHub
* Markdown
* Modern web browser
* Draw.io / Excalidraw / Figma / Microsoft PowerPoint for the cloud infrastructure diagram

## Linux Commands Executed

The following Linux commands were used to investigate the cloud server:

```bash
cat /etc/os-release
uname -r
lscpu
nproc
free -h
df -h
lsblk
hostname
hostname -I
ip addr
```

### Purpose of the Commands

| Command               | Purpose                                                         |
| --------------------- | --------------------------------------------------------------- |
| `cat /etc/os-release` | Displays information about the operating system.                |
| `uname -r`            | Displays the Linux kernel version.                              |
| `lscpu`               | Displays CPU architecture and processor information.            |
| `nproc`               | Displays the number of available processing units.              |
| `free -h`             | Displays memory and RAM information in a readable format.       |
| `df -h`               | Displays disk space and mounted file system information.        |
| `lsblk`               | Displays information about available block devices and storage. |
| `hostname`            | Displays the hostname of the server.                            |
| `hostname -I`         | Displays the IP address assigned to the server.                 |
| `ip addr`             | Displays network interfaces and IP address information.         |

## Skills Learned

During this laboratory, I developed several skills related to cloud computing and Linux administration. I learned how to inspect a Linux server and identify its operating system, kernel, CPU, memory, storage, hostname, and network information. I also learned how compute, storage, networking, operating systems, and identity management contribute to cloud infrastructure.

In addition, I improved my Markdown documentation skills and learned how to organize technical information in a GitHub repository. I also gained experience comparing the infrastructure services of major cloud providers and creating a simple cloud infrastructure diagram.

## Challenges Encountered

One challenge I encountered during this laboratory was understanding the different Linux commands and the type of information returned by each command. Some commands displayed a large amount of information, so I needed to identify the specific details required for the laboratory.

Another challenge was understanding how the different cloud infrastructure components are connected and how similar services are named differently by cloud providers. Organizing the information into Markdown files and maintaining a structured GitHub repository also required careful attention to the required folder and file structure.

Overall, completing these tasks helped me become more comfortable with Linux commands, cloud infrastructure concepts, technical documentation, and GitHub.
