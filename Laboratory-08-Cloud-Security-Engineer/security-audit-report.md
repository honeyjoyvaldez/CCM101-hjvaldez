# Security Audit Report: Chapter 8 Concepts

## The Principle of Least Privilege (PoLP)
The Principle of Least Privilege (PoLP) dictates that users, processes, and systems should only be granted the minimum level of access necessary to perform their required tasks. For cloud user accounts, this is critical because it contains the blast radius of a security breach, preventing attackers from easily moving laterally across other cloud resources if a single account is compromised.

## Attack Surface
The attack surface represents the total sum of all possible entry points, vulnerabilities, and open network ports on a virtual machine that an unauthorized entity could attempt to exploit. When applied to a virtual machine, minimizing the attack surface involves disabling unnecessary services and ports to reduce the avenues available for malicious actors.

## Default Deny Policy
A Default Deny policy is a foundational security posture that blocks all incoming network traffic by default unless an explicit rule permits it[. It is significantly safer than trying to blacklist specific hackers individually because new threats emerge constantly, making it impossible to predict or block every malicious IP address manually[.
```

---

## 2. `firewall-configuration.md`
*(For Checkpoint 6: Technical Documentation)*

```markdown
# Firewall Configuration and Technical Documentation

## Commands Executed
To secure the server using the Uncomplicated Firewall (UFW), the following commands were executed sequentially:

1. **Allow SSH Access:**
   ```bash
   sudo ufw allow ssh
