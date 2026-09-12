# Docker Deployment and Container Lifecycle Documentation

## Checkpoint 3: Environment Setup & Verification
To verify that Docker is properly installed and running in the KillerCoda environment, the following command was executed:
- `docker --version` or `systemctl status docker`

## Checkpoint 4: Deploying Nginx Web Server
To deploy the live web server, the official Nginx image was pulled and executed in detached mode with port mapping:
1. Pull the image: `docker pull nginx`
2. Run container: `docker run -d -p 8080:80 --name my-web-server nginx`
3. Verify locally: `curl http://localhost:8080`

## Checkpoint 5: Container Lifecycle Commands

1. **List running containers:**
   - Command: `docker ps`
   - *Explanation:* Displays all active containers currently running on the host environment, showing their container IDs, status, and port mappings.

2. **Stop the running container:**
   - Command: `docker stop my-web-server`
   - *Explanation:* Gracefully halts the execution of the specified running container process.

3. **Verify it is stopped:**
   - Command: `docker ps -a`
   - *Explanation:* Lists all containers (including stopped ones) to confirm that the container status has changed to "Exited".

4. **Remove the container completely:**
   - Command: `docker rm my-web-server`
   - *Explanation:* Deletes the stopped container instance from disk, freeing up system resources.

