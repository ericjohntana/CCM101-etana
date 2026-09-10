# Laboratory 03 – Multi-Cloud Explorer

## CCM101 – Cloud Computing

This laboratory activity explores three major public cloud providers:

* Amazon Web Services (AWS)
* Microsoft Azure
* Google Cloud Platform (GCP)

The activity focuses on researching cloud platforms, comparing their services, recommending cloud solutions for different business scenarios, and connecting a Linux environment to equivalent cloud computing services.

---

# Checkpoint 1 – Portfolio Structure

The Laboratory 03 folder contains the following files:

```text
Laboratory-03-Multi-Cloud-Explorer/
│
├── README.md
├── aws-research.md
├── azure-research.md
├── gcp-research.md
├── cloud-platform-comparison.md
├── client-recommendations.md
├── reflection.md
│
└── screenshots/
```

---

# Checkpoint 2 – Cloud Platform Research

I researched the following cloud providers:

1. Amazon Web Services
2. Microsoft Azure
3. Google Cloud Platform

The research covered their global infrastructure, management consoles, core services, advantages, and enterprise use cases.

---

# Checkpoint 3 – Cloud Platform Comparison

The three providers were compared based on:

* Launch year
* Compute services
* Storage services
* Networking
* Identity management
* Primary strengths
* Ideal organizations

The detailed comparison is available in:

`cloud-platform-comparison.md`

---

# Checkpoint 4 – Client Recommendations

I analyzed four different business scenarios:

* Startup Company
* University
* AI Research Company
* Global E-Commerce Company

The detailed recommendations are available in:

`client-recommendations.md`

---

# Checkpoint 5 – Service Matching

Equivalent services from AWS, Azure, and Google Cloud were matched for:

* Virtual machines
* Object storage
* Identity management
* SQL databases
* Kubernetes

---

# Checkpoint 6 – Decision Matrix

A cloud decision matrix was created based on different business requirements, including:

* Startup companies
* Enterprise organizations
* Microsoft environments
* AI and machine learning
* Kubernetes
* Global web applications

---

# Checkpoint 7 – Linux Investigation

## Operating System

I used the following command:

```bash
cat /etc/os-release
```

### Result

**Operating System:** `PRETTY_NAME="Ubuntu 24.04.4 LTS"`

---

## CPU Information

I used:

```bash
lscpu
```

### Result

**CPU:** `Intel Xeon E312xx (Sandy Bridge, IBRS update)`

**CPU Cores:** `1`

---

## Memory

I used:

```bash
free -h
```

### Result

**Total Memory:** `1.9Gi`

**Used Memory:** `424Mi`

**Available Memory:** `1.4Gi`

---

## Disk Space

I used:

```bash
df -h
```

### Result

**Total Size:** `19 GB`

**Used:** `5.4 GB`

**Available:** `13 GB`

**Usage:** `30%`

---

# Cloud Migration Possibilities

![KillerCoda Terminal](https://github.com/Jayvie03/CCM101-jlimen/blob/main/Laboratory-03-Multi-Cloud-Explorer/screenshots/checkpoint2-aws-homepage.png)
---

# Cloud Migration Possibilities

If this Linux server were migrated to the cloud, it could be hosted using virtual machine services from each provider.

| Cloud Provider  | Possible Service       |
| --------------- | ---------------------- |
| AWS             | Amazon EC2             |
| Microsoft Azure | Azure Virtual Machines |
| Google Cloud    | Compute Engine         |

These services provide virtual computing environments where a Linux operating system and applications can be hosted.

---

# Conclusion

Laboratory 03 helped me understand that AWS, Azure, and Google Cloud provide similar fundamental cloud capabilities but have different strengths. Comparing the providers helps organizations choose a platform according to their technical requirements, existing infrastructure, budget, scalability requirements, and business objectives.
