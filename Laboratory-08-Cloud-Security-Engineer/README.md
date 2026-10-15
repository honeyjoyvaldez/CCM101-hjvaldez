---

### 2. Contents for `README.md` (inside `Laboratory-08-Cloud-Security-Engineer/`)

Copy and paste this exact content into your folder's `README.md` file:

```markdown
# Laboratory 08: The Cloud Security Engineer

## Mission Overview
As a member of the Cloud Security Team at CloudNova Technologies, this laboratory focuses on applying defense-in-depth principles by locking down an exposed Ubuntu server using a host-based firewall (UFW).

## Objectives
* Understand the concept of the Attack Surface and the Principle of Least Privilege (PoLP).
* Perform a basic security audit of active network ports on a Linux server.
* Configure the Uncomplicated Firewall (UFW) with a Default Deny policy.
* Implement granular port management to selectively allow SSH and HTTP/8080 traffic.
* Document firewall rules and security best practices using Markdown.

## Commands Executed
* `sudo ufw allow ssh`
* `sudo ufw default deny incoming`
* `sudo ufw default allow outgoing`
* `sudo ufw enable`
* `sudo ufw status verbose`
* `sudo ufw allow 8080/tcp`
* `sudo ufw status numbered`

## Skills Learned
* Configuring and managing host-based firewalls using UFW on Linux systems
* Enforcing the Principle of Least Privilege and default-deny networking models.
* Minimizing a server's attack surface by closing unnecessary ports.
* Developing comprehensive technical documentation using Markdown.

