# Infrastructure Assessment Report

## Operating System & Kernel
* **Operating System:** Ubuntu 24.04.4 LTS (Noble Numbat)
* **Kernel Version:** 6.8.0-138-generic

## Compute Resources
* **CPU Model:** Intel Xeon E312xx (Sandy Bridge, IBRS update) @ 2.0GHz
* **Number of CPU Cores:** 1
* **Total RAM:** 1.9 GiB

## Storage & File Systems
* **Disk Capacity:** 19 GiB (Root partition `/dev/vda1`)
* **Mounted File Systems:**
  ```text
  Filesystem      Size  Used Avail Use% Mounted on
  tmpfs           191M  996K  190M   1% /run
  /dev/vda1        19G  5.4G   13G  30% /
  tmpfs           952M   84K  952M   1% /dev/shm
  tmpfs           5.0M     0  5.0M   0% /run/lock
  /dev/vda16      881M  117M  703M  15% /boot
  /dev/vda15      105M  6.2M   99M   6% /boot/efi
