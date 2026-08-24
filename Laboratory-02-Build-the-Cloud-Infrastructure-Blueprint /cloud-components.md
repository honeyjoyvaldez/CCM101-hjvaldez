# Cloud Infrastructure Components Analysis

## 1. Compute Resources
* **Description & Purpose:** Compute resources provide the CPU and RAM necessary to process instructions, execute software applications, and manage dynamic workloads in real time.
* **Importance in Cloud Computing:** Serves as the virtual engine (VMs, containers, serverless functions) allowing organizations to run applications dynamically without provisioning physical server hardware.
* **Linux Environment Mapping:** In the KillerCoda environment, compute is represented by the virtualized Intel Xeon E312xx CPU (1 Core) and 1.9 GiB RAM executing active terminal tasks.

---

## 2. Storage Resources
* **Description & Purpose:** Storage resources save system configuration files, application binaries, database records, and user content persistently or transiently.
* **Importance in Cloud Computing:** Guarantees data durability across instance restarts and provides flexible scaling through block, file, and object storage solutions.
* **Linux Environment Mapping:** Represented by the virtual block storage device `/dev/vda1` (19 GiB capacity) mounted at the root filesystem `/`.

---

## 3. Networking Resources
* **Description & Purpose:** Networking components configure routing rules, domain resolution, and network interfaces that enable secure communication between hosts and client end-users.
* **Importance in Cloud Computing:** Establishes isolated network perimeters (VPCs), manages external access via gateways/firewalls, and enables inter-service data transfer.
* **Linux Environment Mapping:** Represented by the virtual network interface `enp1s0` and its assigned private IP address `172.30.1.2`.

---

## 4. Operating System
* **Description & Purpose:** The operating system acts as the intermediary software layer between application code and hardware, managing memory, process scheduling, and disk input/output.
* **Importance in Cloud Computing:** Provides a standardized execution environment that hosts web servers, database engines, containerization engines, and deployment scripts.
* **Linux Environment Mapping:** Represented by Ubuntu 24.04.4 LTS running Linux kernel version 6.8.0-138-generic in the KillerCoda terminal.
