# Laboratory 5: The Cloud Data Engineer

## Mission Overview
Deployed an S3-compatible object storage server (MinIO) using Docker, accessed its web console, created a bucket named `client-photos`, and uploaded a test file for a photo-sharing client.

## Objectives
- Differentiate between Block, File, and Object Storage
- Deploy an S3-compatible object storage server using Docker
- Access a cloud service through a web interface via port forwarding
- Create a bucket and upload objects
- Document cloud storage operations using Markdown

## Tools Used
- KillerCoda Playground (Ubuntu)
- Docker
- MinIO
- GitHub
- Markdown

## Skills Learned
- Differentiating between block, file, and object storage, and choosing the right type for a given use case
- Deploying an S3-compatible object storage server (MinIO) using a single `docker run` command
- Mapping container ports to the host (`-p 9000:9000 -p 9001:9001`) to expose the API and web console
- Configuring a container at startup using environment variables (`-e`)
- Verifying that a container is running with `docker ps`
- Accessing a service running in a remote environment through KillerCoda's port forwarding
- Creating a storage bucket and uploading objects through the MinIO web console
- Documenting technical configurations and evidence clearly using Markdown
- Organizing lab work in a GitHub repository with commits and pushes after each checkpoint
