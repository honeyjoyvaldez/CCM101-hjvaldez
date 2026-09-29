# Laboratory 06: The Cloud Deployment Engineer

## Mission Overview
CloudNova Technologies assigned a proof-of-concept deployment to migrate a university from third-party storage to a self-hosted enterprise private cloud solution using Nextcloud. Nextcloud requires an underlying database to store metadata and user management records. This project transitions deployment methodologies from manual container management to Infrastructure as Code (IaC) using Docker Compose to orchestrate a two-tier application stack comprising a MariaDB database backend and a Nextcloud frontend web server.

## Objectives
* Explain two-tier and multi-tier cloud application architectures.
* Configure multi-container orchestration blueprints using docker-compose.yml.
* Utilize Linux command-line text editors (nano) for system configuration.
* Deploy, verify, and gracefully terminate container stacks via Docker Compose.
* Document Infrastructure as Code concepts, service routing, and technical reflections using Markdown.

## Commands Executed
```bash
# Create working directory and navigate into it
mkdir nextcloud-deployment
cd nextcloud-deployment

# Open text editor to write configuration code
nano docker-compose.yml

# Deploy multi-container stack in background mode
docker-compose up -d

# Verify status of active containers
docker-compose ps

# Gracefully stop and remove container stack
docker-compose down
