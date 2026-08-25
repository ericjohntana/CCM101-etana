# Cloud Provider Comparison

## Introduction

Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP) are major public cloud providers. They provide equivalent categories of infrastructure services, although the names and implementation of those services can differ. Each provider offers computing, storage, networking, and identity and access management services that organizations can use to build and manage cloud infrastructure.

## Cloud Infrastructure Service Comparison

| Infrastructure Component             | AWS                                      | Microsoft Azure                 | Google Cloud Platform                             |
| ------------------------------------ | ---------------------------------------- | ------------------------------- | ------------------------------------------------- |
| Compute                              | Amazon EC2                               | Azure Virtual Machines          | Compute Engine                                    |
| Storage                              | Amazon S3                                | Azure Blob Storage              | Cloud Storage                                     |
| Networking                           | Amazon VPC                               | Azure Virtual Network (VNet)    | Virtual Private Cloud (VPC)                       |
| Identity and Access Management (IAM) | AWS Identity and Access Management (IAM) | Microsoft Entra ID / Azure RBAC | Google Cloud Identity and Access Management (IAM) |

AWS provides Amazon EC2 for virtual computing, Amazon S3 for object storage, Amazon VPC for virtual networking, and AWS IAM for controlling access to AWS resources.

Google Cloud provides Compute Engine for virtual machines, Cloud Storage for storage, VPC for networking, and Cloud IAM for managing identities, roles, and permissions.

Azure provides Azure Virtual Machines for computing, Azure Blob Storage for object storage, Azure Virtual Network for networking, and Microsoft Entra ID together with Azure RBAC for identity and access control. Microsoft documentation describes Entra ID as supporting authorization to Blob data and Azure RBAC as a way to grant access rights.

## Guide Questions

### 1. Which cloud provider offers the broadest range of services?

AWS is widely recognized for having one of the broadest selections of cloud services. It provides services covering computing, storage, networking, databases, security, analytics, artificial intelligence, and many other areas.

### 2. Which cloud platform would you recommend for an organization that primarily uses Microsoft products? Why?

Microsoft Azure would be a strong recommendation for an organization that primarily uses Microsoft products. Azure integrates closely with Microsoft's technologies and identity services, which can make it easier for organizations already using Microsoft environments to manage their cloud resources.

### 3. Which platform is widely recognized for Artificial Intelligence (AI), Machine Learning (ML), and Kubernetes services?

Google Cloud is widely recognized for its strengths in Artificial Intelligence, Machine Learning, and Kubernetes. Google Cloud also provides Google Kubernetes Engine (GKE), while its cloud platform includes services and tools designed for AI and machine-learning workloads.

### 4. What similarities did you observe among the three cloud providers?

The three cloud providers offer similar fundamental infrastructure categories, including compute, storage, networking, and identity and access management. Although the service names and specific features differ, all three platforms allow organizations to provision resources, manage access, store data, and connect cloud resources through virtual networks.

## Conclusion

AWS, Microsoft Azure, and Google Cloud Platform provide comparable categories of cloud infrastructure services. Although their service names and specific features differ, all three provide computing, storage, networking, and identity-related capabilities. Understanding the equivalent services makes it easier for cloud engineers to compare platforms and choose an appropriate provider for an organization's requirements.
