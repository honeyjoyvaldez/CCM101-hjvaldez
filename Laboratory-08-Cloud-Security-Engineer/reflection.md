---

## 3. `reflection.md`
*(For Checkpoint 7: Mission Reflection)*

```markdown
# Mission Reflection: Cloud Security Engineer

A host-based firewall protects a server even if the physical or outer network perimeter is breached by locally inspecting and filtering traffic at the operating system level, ensuring that individual virtual machines maintain strict isolation and access control[cite: 3, 4]. Managing open network ports is critical to reducing a server's attack surface because every active port represents a potential entry vector that can be leveraged by attackers to exploit running services. 

In a real enterprise environment, leaving a database port like 3306 for MySQL open to the public internet is extremely dangerous because it exposes backend data stores directly to automated brute-force attacks, credential stuffing, and potential remote code execution. Completing this mission changed my perspective by highlighting how rapidly an unconfigured server can become completely exposed and vulnerable the moment it connects to the internet, proving that security requires intentional, proactive hardening rather than passive assumptions. 

Looking at my GitHub portfolio with eight completed missions, I feel a strong sense of accomplishment. The repository has evolved into a comprehensive, structured record of core cloud engineering proficiencies spanning infrastructure blueprints, native deployments, operations, and now cloud security.
```

---

## 4. `README.md`
*(For `Laboratory-08-Cloud-Security-Engineer/`)*

```markdown
# Laboratory 08: The Cloud Security Engineer

## Mission Overview
As part of the Cloud Security Team at CloudNova Technologies, this laboratory focuses on applying defense-in-depth principles by locking down an exposed Ubuntu server using a host-based firewall (UFW).

## Objectives
* Understand the attack surface and the Principle of Least Privilege (PoLP).
* Perform a basic security audit of active network ports.
* Configure UFW with a Default Deny policy and granular port management.
* Document firewall configurations and security best practices using Markdown.

## Directory Structure
```text
Laboratory-08-Cloud-Security-Engineer/
├── README.md
├── security-audit-report.md
├── firewall-configuration.md
├── reflection.md
└── screenshots/
    ├── vulnerable-app-running.png
    ├── firewall-activated.png
    └── firewall-port-allowed.png
