# Types of Cloud Storage

| Storage Type | Description (How it stores data) | Primary Use Case | Cloud Provider Example |
|--------------|----------------------------------|------------------|------------------------|
| **Block Storage** | Splits data into fixed-size blocks, each with its own address. Attached to a server like a hard drive, so the operating system formats it and manages the files on it. | Operating system disks, databases, and applications that need fast, low-latency reads and writes. | AWS EBS (Elastic Block Store) |
| **File Storage** | Stores data as files in a hierarchy of folders and paths. Shared over a network using protocols like NFS or SMB, so many servers can access the same files at once. | Shared drives, home directories, content management, and applications that need a common file system. | AWS EFS (Elastic File System) |
| **Object Storage** | Stores each item as an object: the data itself, its metadata, and a unique ID, all in a flat structure (no folders on disk). Accessed over HTTP through an API. | Images, videos, backups, logs, and other large amounts of unstructured data. | AWS S3 (Simple Storage Service) |

## Why Object Storage for the Client's Photos

Object storage is the best fit for your photo-sharing application because it can grow to millions of images without you managing disks or servers, and you only pay for the storage you use. Each photo is stored as an independent object with its own metadata and unique ID, so it can be retrieved directly over the web by your app. It is also more durable than a container's local storage, because your images stay safe even when a web server container is restarted or replaced.

## References

- AWS. "What is Block Storage?" https://aws.amazon.com/what-is/block-storage/
- AWS. "What is Object Storage?" https://aws.amazon.com/what-is/object-storage/
- AWS. "What is File Storage?" https://aws.amazon.com/what-is/file-storage/
