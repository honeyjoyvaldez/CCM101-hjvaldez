# System Baseline Report

**Course:** CCM101 - Cloud Computing  
**Lab:** Mission 7 - The Cloud Operations Engineer  

---

## 1. Host Performance Diagnostics

Native Linux CLI tools were used to establish a baseline health check on the host server prior to generating synthetic application traffic:

* `free -h` - Measured physical RAM availability and allocation.
* `df -h` - Inspected storage capacity on the root (`/`) filesystem.
* `top` - Analyzed running processes and dynamic CPU load metrics.

---

## 2. Server Resource Baseline Data

* **Total RAM Available:** `1.9Gi`
* **Root File System Capacity:** `19G`

---

## 3. Operational Analysis

### Criticality of Disk Space Monitoring
Checking available disk space before a massive traffic surge is critical because web applications constantly write access logs, error logs, and temporary cache files; exhausting disk space will cause database write failures, application runtime crashes, and complete service outages.
