---

### File 3: `README.md`

```markdown
# Laboratory 07: The Cloud Operations Engineer

## Mission Overview
As a Cloud Operations / Site Reliability Engineer (SRE) at CloudNova Technologies, this mission focused on establishing infrastructure baseline health, deploying containerized application workloads, generating synthetic web traffic, and analyzing runtime metrics and logs.

## Objectives
* Monitor host CPU, Memory, and Disk capacity using native Linux commands.
* Deploy an Nginx container and monitor live resource utilization using Docker metrics.
* Generate HTTP traffic, simulate HTTP 404 errors, and extract application logs.
* Document operational health data in structured Markdown technical reports.

## Monitoring Commands Executed
| Command | Category | Purpose |
| :--- | :--- | :--- |
| `free -h` | Host Diagnostics | Inspects server RAM capacity and available memory[. |
| `df -h` | Host Diagnostics | Checks storage usage and root filesystem capacity. |
| `top` | Host Diagnostics | Displays dynamic CPU load and active running processes. |
| `docker run -d -p 8080:80 --name client-website nginx` | Deployment | Deploys Nginx container in background mode on port 8080. |
| `curl http://localhost:8080` | Synthetic Traffic | Sends successful HTTP GET requests (HTTP 200). |
| `curl http://localhost:8080/hidden-admin-page` | Error Generation | Triggers an intentional 404 Not Found error. |
| `docker logs client-website` | Observability | Fetches container access and error logs[cite: 3. |
| `docker stats client-website` | Observability | Displays streaming real-time CPU, Memory, and I/O metrics. |

## Skills Learned
* Establishing server hardware performance baselines.
* Using container log streams to track user requests and error status codes.
* Real-time resource monitoring for containerized microservices.
* Translating raw terminal monitoring output into technical reports.
