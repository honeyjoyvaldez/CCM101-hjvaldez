# Mission Reflection

The boot time and setup process of a Docker container are drastically faster and lighter compared to installing an operating system on a traditional Virtual Machine. While a VM requires minutes to boot up because it initializes an entire guest OS kernel, system services, and virtual hardware, a Docker container launches in mere seconds by sharing the host machine's OS kernel and executing as an isolated user-space process.

Port mapping, such as `-p 8080:80`, is necessary because containers operate in an isolated network namespace. Without explicit mapping, the web server listening on port 80 inside the container remains unreachable from outside network interfaces. Port mapping creates a network bridge that routes external traffic from port 8080 on the host machine directly to port 80 inside the container.

When you execute the `docker rm` command, the specified container instance is deleted along with its writable container layer. Any temporary files or application data written inside the container during runtime are permanently lost unless explicitly backed up or persisted using Docker volumes or bind mounts.

Containerization fundamentally transforms how software developers and IT operations teams collaborate within DevOps. By packaging applications alongside their exact dependencies into immutable container images, developers ensure consistency across development, testing, and production environments. This eliminates the traditional "it works on my machine" issue and enables operations teams to automate deployment pipelines efficiently.

Finally, maintaining and evolving this GitHub portfolio serves as a practical record of my growth in cloud-native technologies. It reinforces technical documentation best practices and demonstrates hands-on competency in container orchestration and cloud architecture.
