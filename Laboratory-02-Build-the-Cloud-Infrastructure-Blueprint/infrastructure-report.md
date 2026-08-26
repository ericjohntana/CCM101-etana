# Infrastructure Report

## 1. Operating System

| Information      | Value                      |
| ---------------- | -------------------------- |
| Operating System | Ubuntu                     |
| Pretty Name      | Ubuntu 24.04.4 LTS         |
| Version ID       | 24.04                      |
| Version          | 24.04.4 LTS (Noble Numbat) |
| Version Codename | noble                      |
| ID               | ubuntu                     |
| ID Like          | debian                     |
| Ubuntu Codename  | noble                      |
| Logo             | ubuntu-logo                |

## 2. Kernel Version

| Information  | Value                        |
| ------------ | ---------------------------- |
| Kernel       | Linux 6.8.0-138-generic      |
| Build        | #138-Ubuntu                  |
| Architecture | x86_64                       |
| SMP          | PREEMPT_DYNAMIC              |
| Build Date   | Fri Jul 31 22:41:49 UTC 2026 |

## 3. CPU Model

| Information         | Value                                         |
| ------------------- | --------------------------------------------- |
| Architecture        | x86_64                                        |
| CPU Mode            | 32-bit, 64-bit                                |
| Address Sizes       | 39 bits physical, 48 bits virtual             |
| Byte Order          | Little Endian                                 |
| CPU(s)              | 1                                             |
| Vendor ID           | GenuineIntel                                  |
| BIOS Vendor         | Red Hat                                       |
| Model Name          | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| BIOS Model          | RHEL-9.6.0 PC (Q35 + ICH9, 2009) CPU @ 2.0GHz |
| CPU Family          | 6                                             |
| Model               | 42                                            |
| Thread(s) per Core  | 1                                             |
| Core(s) per Socket  | 1                                             |
| Socket(s)           | 1                                             |
| Stepping            | 1                                             |
| BogoMIPS            | 7008.00                                       |
| Hypervisor Vendor   | KVM                                           |
| Virtualization Type | Full                                          |

### CPU Cache

| Cache |   Size |
| ----- | -----: |
| L1d   | 32 KiB |
| L1i   | 32 KiB |
| L2    |  4 MiB |
| L3    | 16 MiB |

### NUMA Information

| Information        | Value |
| ------------------ | ----- |
| NUMA Node(s)       | 1     |
| NUMA Node 0 CPU(s) | 0     |

## 4. CPU Cores

| Information                | Value |
| -------------------------- | ----: |
| Number of CPU Cores        |     1 |
| Available Processing Units |     1 |

## 5. Total RAM

| Memory |   Total |    Used |    Free |  Shared | Buff/Cache | Available |
| ------ | ------: | ------: | ------: | ------: | ---------: | --------: |
| RAM    | 1.9 GiB | 430 MiB | 852 MiB | 1.1 MiB |    788 MiB |   1.4 GiB |
| Swap   | 1.0 GiB |     0 B | 1.0 GiB |       — |          — |         — |

## 6. Disk Capacity

| Filesystem   | Size | Used | Available | Use % | Mounted On  |
| ------------ | ---: | ---: | --------: | ----: | ----------- |
| tmpfs        | 191M | 996K |      190M |    1% | `/run`      |
| `/dev/vda1`  |  19G | 5.4G |       13G |   30% | `/`         |
| tmpfs        | 952M |  84K |      952M |    1% | `/dev/shm`  |
| tmpfs        | 5.0M |    0 |      5.0M |    0% | `/run/lock` |
| `/dev/vda16` | 881M | 117M |      703M |   15% | `/boot`     |
| `/dev/vda15` | 105M | 6.2M |       99M |    6% | `/boot/efi` |

## 7. Mounted File Systems

| Filesystem   | Mount Point                | Type        | Options                                         |
| ------------ | -------------------------- | ----------- | ----------------------------------------------- |
| sysfs        | `/sys`                     | sysfs       | rw,nosuid,nodev,noexec,relatime                 |
| proc         | `/proc`                    | proc        | rw,nosuid,nodev,noexec,relatime                 |
| udev         | `/dev`                     | devtmpfs    | rw,nosuid,relatime                              |
| devpts       | `/dev/pts`                 | devpts      | rw,nosuid,noexec,relatime                       |
| tmpfs        | `/run`                     | tmpfs       | rw,nosuid,nodev,noexec,relatime                 |
| `/dev/vda1`  | `/`                        | ext4        | rw,relatime,discard,errors=remount-ro,commit=30 |
| securityfs   | `/sys/kernel/security`     | securityfs  | rw,nosuid,nodev,noexec,relatime                 |
| tmpfs        | `/dev/shm`                 | tmpfs       | rw,nosuid,nodev,inode64                         |
| tmpfs        | `/run/lock`                | tmpfs       | rw,nosuid,nodev,noexec,relatime                 |
| cgroup2      | `/sys/fs/cgroup`           | cgroup2     | rw,nosuid,nodev,noexec,relatime                 |
| pstore       | `/sys/fs/pstore`           | pstore      | rw,nosuid,nodev,noexec,relatime                 |
| bpf          | `/sys/fs/bpf`              | bpf         | rw,nosuid,nodev,noexec,relatime                 |
| systemd-1    | `/proc/sys/fs/binfmt_misc` | autofs      | rw,relatime                                     |
| hugetlbfs    | `/dev/hugepages`           | hugetlbfs   | rw,nosuid,nodev,relatime                        |
| mqueue       | `/dev/mqueue`              | mqueue      | rw,nosuid,nodev,noexec,relatime                 |
| debugfs      | `/sys/kernel/debug`        | debugfs     | rw,nosuid,nodev,relatime                        |
| tracefs      | `/sys/kernel/tracing`      | tracefs     | rw,nosuid,nodev,relatime                        |
| fusectl      | `/sys/fs/fuse/connections` | fusectl     | rw,nosuid,nodev,relatime                        |
| configfs     | `/sys/kernel/config`       | configfs    | rw,nosuid,nodev,relatime                        |
| `/dev/vda16` | `/boot`                    | ext4        | rw,relatime                                     |
| `/dev/vda15` | `/boot/efi`                | vfat        | rw,relatime                                     |
| binfmt_misc  | `/proc/sys/fs/binfmt_misc` | binfmt_misc | rw,nosuid,nodev,noexec,relatime                 |

## 8. Hostname

| Information | Value    |
| ----------- | -------- |
| Hostname    | `ubuntu` |

## 9. IP Address

| Type         | IP Address   |
| ------------ | ------------ |
| IP Address 1 | `172.30.1.2` |
| IP Address 2 | `172.17.0.1` |

## Linux Commands Used

| Command               | Purpose                                                 |
| --------------------- | ------------------------------------------------------- |
| `cat /etc/os-release` | Displays operating system information.                  |
| `uname -a`            | Displays detailed kernel and system information.        |
| `lscpu`               | Displays CPU architecture and processor information.    |
| `nproc`               | Displays the number of available processing units.      |
| `free -h`             | Displays RAM and swap memory information.               |
| `df -h`               | Displays disk space and mounted filesystem information. |
| `lsblk`               | Displays information about block devices and storage.   |
| `hostname`            | Displays the hostname of the server.                    |
| `hostname -I`         | Displays the IP addresses assigned to the system.       |
| `ip addr`             | Displays network interfaces and IP address information. |
