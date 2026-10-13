# MinIO Object Storage Deployment

## 1. Overview

In this laboratory activity, I deployed MinIO, an S3-compatible object storage server, using Docker in the KillerCoda Ubuntu Playground. The purpose was to create an object storage environment for a photo-sharing application and prepare to store uploaded images in a bucket.

## 2. Environment and Tools

- **Environment:** KillerCoda Ubuntu Playground
- **Container Platform:** Docker
- **Object Storage Server:** MinIO
- **Container Name:** `minio-server`
- **Docker Image:** `chainguard/minio:latest`
- **API Port:** `9000`
- **Web Console Port:** `9001`

## 3. Check Docker Installation

I checked the installed Docker version using the following command:

```bash
docker --version
```

The terminal displayed Docker version `29.1.3`.

## 4. Deploy MinIO Using Docker

The original image specified in the laboratory handout, `minio/minio`, returned an access-denied error. I therefore used the alternative image `chainguard/minio:latest`.

The Docker command I used was:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" chainguard/minio:latest server /data --console-address ":9001"
```

### Explanation of the Docker Command

- `docker run` creates and starts a container.
- `-d` runs the container in the background.
- `-p 9000:9000` maps port 9000 for the MinIO API.
- `-p 9001:9001` maps port 9001 for the MinIO Web Console.
- `--name minio-server` assigns a name to the container.
- `chainguard/minio:latest` specifies the Docker image.
- `server /data` starts MinIO using `/data` as its storage directory.
- `--console-address ":9001"` configures the Web Console to listen on port 9001.

### Environment Variables

The `-e` flag passes environment variables to the container.

- `MINIO_ROOT_USER=cloudadmin` sets the MinIO root username.
- `MINIO_ROOT_PASSWORD=CloudNova2026!` sets the MinIO root password.

These credentials were configured for this laboratory deployment.

## 5. Verify the Container

I used the following command to check whether the container was running:

```bash
docker ps
```

The output showed the container named `minio-server` with a status of `Up` and port mappings for `9000` and `9001`.

## 6. Access the MinIO Web Console

The Web Console uses port `9001`.

To access it, I followed these steps:

1. Open the KillerCoda Playground.
2. Locate the Traffic / Ports or Custom Ports section.
3. Enter port `9001` and click Access.
4. Sign in using the configured laboratory credentials.

## 7. Create the Bucket and Upload a File

The required bucket name for this activity is `client-photos`.

After accessing the MinIO Web Console, the steps are:

1. Navigate to Buckets.
2. Click Create Bucket.
3. Enter `client-photos` and save it.
4. Open the bucket.
5. Upload a sample image or text file.
6. Verify that the uploaded file appears in the bucket.

## 8. Screenshots and Evidence

The required screenshots for this activity are:

- `screenshots/minio-deployed.png` — Shows the MinIO deployment and running container in the terminal.
- `screenshots/minio-bucket-upload.png` — Shows the `client-photos` bucket and uploaded file in the Web Console.

## 9. Result

The MinIO container was deployed successfully using Docker in the KillerCoda Playground. The terminal confirmed that the container was running and ports 9000 and 9001 were mapped.

## 10. Conclusion

This activity provided hands-on experience deploying MinIO and verifying the container through the terminal. It also introduced the use of object storage for cloud-based file storage.

