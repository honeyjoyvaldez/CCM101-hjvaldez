# Laboratory Activity 02: Build the Cloud Infrastructure Blueprint

## Mission Overview
The objective of this laboratory activity is to inspect, document, and map out a cloud-hosted Linux environment. By auditing the system resources of a KillerCoda virtual instance, mapping core Linux primitives to cloud infrastructure components, comparing major cloud service providers (AWS, Azure, GCP), and creating an architectural diagram, this blueprint establishes a comprehensive foundational understanding of cloud environments.

## Objectives
* Investigate and document host metrics (OS, CPU, Memory, Disk, Network) of an active Linux server.
* Map fundamental Linux system components to core cloud computing resources.
* Research and contrast equivalent core infrastructure offerings across AWS, Microsoft Azure, and GCP.
* Design a clear architectural diagram representing a simple enterprise cloud topology.
* Document technical findings, command execution, and learning reflections in standard Markdown.

## Cloud Infrastructure Components
* **Compute:** Represented by the virtualized Intel Xeon E312xx CPU (1 Core) and 1.9 GiB RAM handling process execution.
* **Storage:** Represented by the virtual block device `/dev/vda1` (19 GiB total capacity) mounted at the root directory `/`.
* **Networking:** Represented by the virtual network interface `enp1s0` assigned to private IP address `172.30.1.2`.
* **Operating System:** Represented by Ubuntu 24.04.4 LTS running Linux kernel version `6.8.0-138-generic`.

## Tools Used
* **KillerCoda Terminal:** Web-based interactive Linux environment (Ubuntu 24.04.4 LTS).
* **GitHub:** Repository host for structured Markdown documentation and image asset management.
* **Diagramming Tool (Draw.io / Excalidraw / PPT):** Created the cloud network blueprint export (`cloud-architecture.png`).

## Linux Commands Executed
* `cat /etc/os-release`: Extracted operating system distribution details.
* `uname -r`: Identified active Linux kernel release version.
* `lscpu`: Queried central processing unit architecture and core count.
* `free -h`: Examined total, used, and available system memory (RAM).
* `df -h`: Displayed disk storage usage and filesystem mount paths.
* `hostname`: Outputted system network hostname identification.
* `ip a`: Displayed active network interface adapters and IP addresses.

## Skills Learned
* Shell diagnostics and hardware resource auditing using native Linux CLI tools.
* Translation of low-level OS components to high-level cloud abstractions (Compute, Storage, Networking, OS).
* Comparative analysis of cloud service vendor naming schemes across AWS, Azure, and GCP.
* Technical documentation practices using Git, GitHub, and GitHub-Flavored Markdown.

## Challenges Encountered
* **Formatting Command Outputs:** Running multiple commands separately caused terminal scrollback that obscured comprehensive screen captures. *Resolution:* Used command chaining (`cat /etc/os-release | grep PRETTY_NAME; uname -r; lscpu | grep "Model name\|CPU(s):"; free -h`) to capture all server information in a single screen.
* **Directory Naming Conventions:** Managing strict folder naming without accidental spaces in GitHub paths. *Resolution:* Refactored folder paths directly via GitHub's file view interface to ensure seamless repository organization.
