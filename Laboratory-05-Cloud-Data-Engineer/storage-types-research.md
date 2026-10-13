# Research: Types of Cloud Storage

## Introduction

Cloud storage allows users and applications to save and access data using storage infrastructure. The three primary types of cloud storage are Block Storage, File Storage, and Object Storage. Each type has different characteristics and uses.

## Comparison of Cloud Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in fixed-sized blocks that can be managed as disk volumes. | Virtual machine disks, operating systems, and databases. | Amazon Elastic Block Store (Amazon EBS) |
| File Storage | Stores data as files arranged in folders and directories. | Shared folders, documents, and applications requiring a shared file system. | Amazon Elastic File System (Amazon EFS) |
| Object Storage | Stores data as objects containing the data, metadata, and a unique identifier. Objects are organized into buckets. | Photos, videos, backups, and other unstructured data. | Amazon Simple Storage Service (Amazon S3) |

## Why Object Storage Is Best for the Client

Object Storage is a good choice for the client's photo-sharing application because it is designed to store large amounts of unstructured data, including user-uploaded images. Images can be organized as objects inside buckets, and the storage system can grow as the application receives more photos. It also separates image storage from the web server, helping the application avoid relying on the container's temporary writable storage for its image collection.


