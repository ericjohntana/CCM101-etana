# The Cloud Data Engineer

## Laboratory Overview

This laboratory activity focuses on cloud storage technologies and deploying MinIO using Docker. The activity is performed in the KillerCoda Ubuntu Playground, where Docker is used to run the MinIO object storage server.

The laboratory introduces three types of cloud storage: Block Storage, File Storage, and Object Storage. It also provides hands-on experience deploying a storage service, accessing the MinIO Web Console, and organizing files using a storage bucket.

## Objectives

The objectives of this laboratory activity are to:

- Understand the differences between Block Storage, File Storage, and Object Storage.
- Identify suitable storage types for different cloud computing applications.
- Deploy MinIO using Docker in an Ubuntu environment.
- Verify the MinIO container using Docker commands.
- Access the MinIO Web Console through the assigned port.
- Create a bucket named `client-photos`.
- Upload a sample file to the bucket.
- Document the activity and results in GitHub using Markdown.

## Tools and Technologies Used

| Tool | Purpose |
|---|---|
| KillerCoda Ubuntu Playground | Provides the Linux terminal environment for the laboratory. |
| Docker | Runs MinIO inside a container. |
| MinIO | Provides object storage for files and other unstructured data. |
| GitHub | Stores the laboratory documentation and evidence. |
| Markdown | Formats the laboratory report and project documentation. |

## Laboratory Activities

### Checkpoint 1 — Research Cloud Storage Types

The first checkpoint focuses on understanding the three main cloud storage types: Block Storage, File Storage, and Object Storage. Each type organizes and manages data differently and is suitable for different workloads.

The research and comparison are documented in `storage-types-research.md`.

### Checkpoint 2 — Identify the Appropriate Storage Solution

Object Storage is a suitable option for applications that need to store large collections of photos, videos, backups, and other unstructured data. It organizes data as objects within buckets, making it practical for applications that manage many files.

The storage research helps explain why Object Storage is appropriate for a photo-sharing application.

### Checkpoint 3 — Deploy MinIO Using Docker

MinIO was deployed in the KillerCoda Ubuntu Playground using Docker. The `chainguard/minio:latest` image was used for the deployment after the originally specified `minio/minio` image could not be pulled in the environment.

The container was configured to use ports `9000` and `9001`. Port `9000` is used for the MinIO API, while port `9001` is used for the Web Console.

The deployment was checked through the terminal to verify the container status and port mappings.

The deployment procedure is documented in `minio-deployment.md`.

### Checkpoint 4 — Access the MinIO Web Console

After deploying the container, the next step is to access the MinIO Web Console through port `9001` using the KillerCoda port-access feature.

The configured login credentials are used to sign in to the console. Once access is confirmed, the required bucket can be created and a sample file can be uploaded.

**Required bucket name:** `client-photos`

The deployment and bucket-upload screenshots should be saved in the `screenshots` folder as evidence of the completed activity.

### Checkpoint 5 — Write the Laboratory Reflection

The final checkpoint is to reflect on the laboratory experience, including the cloud storage concepts learned, the Docker deployment process, and the challenges encountered during the activity.

The reflection is documented in `reflection.md`.

## Repository Structure

The laboratory files should follow this structure:

```text
Laboratory-05-Cloud-Data-Engineer/
├── README.md
├── storage-types-research.md
├── minio-deployment.md
├── reflection.md
└── screenshots/
    ├── minio-deployed.png
    └── minio-bucket-upload.png
```

## Expected Evidence

| Evidence File | Description |
|---|---|
| `minio-deployed.png` | Screenshot of the terminal showing the MinIO container status and port mappings. |
| `minio-bucket-upload.png` | Screenshot of the MinIO Web Console showing the `client-photos` bucket and the uploaded sample file. |

Only include screenshots after you have captured them. The bucket-upload screenshot should be taken after the bucket and file have been successfully created and uploaded.

## Skills Developed

Through this activity, I developed and practiced the following skills:

- Understanding cloud storage concepts.
- Using Linux command-line tools.
- Deploying a container with Docker.
- Checking container status and port mappings.
- Learning the basic workflow of MinIO object storage.
- Organizing technical documentation using Markdown.
- Recording laboratory evidence in GitHub.
- Identifying and troubleshooting deployment errors.

## Conclusion

This laboratory activity introduced the differences between Block Storage, File Storage, and Object Storage and demonstrated how Docker can be used to deploy MinIO in a Linux environment. It also provided an opportunity to practice checking container status, configuring ports, and preparing an object storage bucket.

The activity strengthened my understanding of cloud storage and container deployment. Completing the Web Console and bucket-upload steps will provide additional practical experience with storing and managing files through MinIO.

