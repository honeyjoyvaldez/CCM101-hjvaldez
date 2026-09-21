# Mission Reflection

**1. Why is object storage better suited for storing millions of photos than a traditional block storage hard drive?**
Block storage works like a hard drive attached to a single server, so capacity has to be provisioned and managed, and it doesn't scale easily. Object storage keeps each photo as an independent object with its own metadata and unique ID in a flat structure. It can grow almost without limit, and each photo can be retrieved directly over HTTP. It is also usually cheaper for large amounts of unstructured data.

**2. How did using Docker make it easier to deploy the MinIO storage server?**
Without Docker, I would have had to install MinIO and its dependencies on the machine and configure everything by hand. With Docker, a single `docker run` command downloaded the image, started the server, mapped the ports, and set the login credentials. Because the container is self-contained, the setup should work the same on any machine.

**3. What is a "bucket" in the context of cloud storage?**
A bucket is a top-level container that holds objects in object storage, a bit like a main folder. It is where settings such as the name and access permissions are managed. In this lab, the `client-photos` bucket held my uploaded test file.

**4. How do large enterprise companies ensure their object storage data is not lost if a physical server crashes?**
I think they store multiple copies of each object across different disks, servers, and even data centers or regions. Techniques like replication and erasure coding let the system rebuild data if a drive or server fails, and regular backups add another layer of protection.

**5. How is your confidence in navigating the Linux command line growing?**
My confidence is growing steadily. In this lab I used commands like `docker run` and `docker ps` to deploy and verify the MinIO server, and they felt much less intimidating than when I started the course. I now understand what the flags in a long command do, such as `-p` for ports and `-e` for environment variables, instead of just copying and pasting. I still want to get better at troubleshooting with tools like `docker logs`, and at working faster without checking my notes.
