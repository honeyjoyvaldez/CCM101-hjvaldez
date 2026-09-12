# Laboratory Activity 4: The Cloud-Native Engineer

## Mission Overview
Successfully transitioned from traditional virtual machines to containerized cloud architectures at CloudNova Technologies using Docker and the KillerCoda playground environment.

## Objectives
* Differentiate between traditional Virtual Machines (VMs) and Containers.
* Access a Docker-enabled cloud environment using KillerCoda.
* Execute fundamental Docker CLI commands.
* Pull, run, manage, and terminate a containerized Nginx application.
* Create professional technical documentation using Markdown.

## Docker Commands Executed
* `docker --version`
* `docker pull nginx`
* `docker run -d -p 8080:80 --name my-web-server nginx`
* `curl http://localhost:8080`
* `docker ps`
* `docker stop my-web-server`
* `docker ps -a`
* `docker rm my-web-server`

## Skills Learned
* Understanding process-level isolation versus hypervisor-level virtualization.
* Managing container lifecycles via the Docker command-line interface.
* Exposing internal container ports to host ports for external web traffic access.

## Challenges Encountered
Ensuring proper port binding syntax (`-p host_port:container_port`) to ensure local curl requests successfully reached the Nginx server inside the isolated container layer.
