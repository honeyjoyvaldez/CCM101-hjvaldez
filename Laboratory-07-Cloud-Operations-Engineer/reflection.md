# Mission Reflection: Cloud Operations & Observability

### 1. Host Server Resource Monitoring
Even when containers run smoothly, they share the host kernel and underlying hardware resources. If host RAM or root disk space becomes depleted, the host kernel may invoke Out-Of-Memory (OOM) processes or restrict disk writes, silently crashing container environments.

### 2. Troubleshooting Login Failures via `docker logs`
When a user reports login failures, running `docker logs` exposes runtime exceptions, backend failure traces, or HTTP status codes (such as HTTP 500 server errors or HTTP 401/403 authentication failures). This isolates whether the issue lies in backend logic, database timeout issues, or invalid user inputs.

### 3. Log Monitoring vs. Metric Monitoring
* **Logs** detail discrete execution events, error traces, and request paths (explaining **what** happened and **why**).
* **Metrics** track aggregated numerical data over time such as CPU %, memory footprint, and bandwidth usage (explaining **how much** resource headroom remains).

### 4. Enterprise-Scale Observability Architecture
Large enterprise organizations managing thousands of microservices use centralized telemetry stacks. Metrics are scraped and aggregated using **Prometheus** and visualized on dashboards using **Grafana**. Logs are continuously gathered across clusters using central logging aggregators (e.g., Fluentd, ElasticSearch, Logstash).

### 5. Growth in Linux Troubleshooting Capabilities
My troubleshooting capabilities improved by adopting an evidence-based approach—pairing hardware level commands (`top`, `df`, `free`) with container telemetry (`docker logs`, `docker stats`) to diagnose bottlenecks systematically.
