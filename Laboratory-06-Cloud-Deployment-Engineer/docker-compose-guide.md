
# Docker Compose Technical Guide

## 1. The Role of the services: Block
The services: block defines the individual containerized application components that make up the multi-container stack. Under this block, each named service (e.g., database and app) specifies its base container image, environment variables, port mappings, and runtime configurations. Docker Compose reads this block to instantiate, configure, and connect each container into a unified application stack.

## 2. Container Service Discovery (MYSQL_HOST)
The Nextcloud application container locates the MariaDB database container through Docker's built-in internal DNS service discovery. In the docker-compose.yml file, the environment variable MYSQL_HOST is set to database, matching the exact service name defined under services:. When Nextcloud initiates a connection, Docker automatically resolves the service hostname database to the private IP address of the MariaDB container within the shared default container network.

## 3. docker run vs. docker-compose up -d

| Feature | docker run | docker-compose up -d |
| :--- | :--- | :--- |
| *Scope* | Manages a single container per command execution. | Manages an entire multi-container stack simultaneously. |
| *Method* | Imperative; requires typing long CLI arguments and flags. | Declarative; reads stack specifications from a YAML file. |
| *Networking* | Requires manually creating networks and linking containers. | Automatically creates a private network and links all defined services. |
| *Execution* | Runs interactively or requires manual flag management (-d). | Runs all stack services in detached background mode effortlessly (-d). |
| *Maintainability* | Difficult to track, document, or replicate consistently. | Version-controlled Infrastructure as Code (IaC) file. |
