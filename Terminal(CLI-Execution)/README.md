# 💻 Confluent CLI Terminal Execution Log

This directory archives my practical hands-on experience using the command-line interface (CLI) to configure and operate **Confluent Cloud Kafka** directly from a Windows PowerShell terminal. 

These 10 execution checkpoints showcase a complete administrative lifecycle: authenticating, creating environments and clusters, provisioning API security, and executing live terminal-to-terminal data streaming loops.

---

## 🔐 Step 1: Authentication & Cluster Discovery

### Cloud Login Checkpoint
Initiated connection using the `--save` parameter to authenticate the session securely via the web browser environment. The terminal verifies active account details and trial credit statuses.

![Cloud Login Checkpoint](./ss/Screenshot%202026-08-09%20151117.png)

### Automated Environment Provisioning
Created a dedicated resource sandbox environment named `environment_from_cli` directly from the command prompt. The system logs the unique environment metadata and default governance configurations.

![Automated Environment Provisioning](./ss/Screenshot%202026-08-09%20151837.png)

---

## ☁️ Step 2: Infrastructure Deployment via CLI

### Cloud Console Synchronization
A verified visual checkpoint inside the Confluent Web UI showing the workspace configurations updating instantly on the cloud. The platform displays the freshly initialized environment alongside existing profiles.

![Cloud Console Synchronization](./ss/Screenshot%202026-08-09%20152024.png)

### Provisioning a Managed Kafka Cluster
Executed an infrastructure deployment command to spin up a live basic Kafka cluster named `cli_cluster` on AWS (`us-east-1`). The deployment configurations outline structural storage limits and server endpoints.

![Provisioning a Managed Kafka Cluster](./ss/Screenshot%202026-08-09%20152338.png)

### Live Cluster Status Audit
A web dashboard checkpoint verifying that the newly requested cluster has successfully finished its deployment cycles and is officially active on the cloud infrastructure.

![Live Cluster Status Audit](./ss/Screenshot%202026-08-09%20152419.png)

---

## 🛠️ Step 3: Topic Design & Security Credentialing

### Resource Selection & Topic Mapping
Targeted the active cluster environment and initialized a fresh data topic named `customer_transaction` with a custom replication factor and partitioned logging parameters.

![Resource Selection & Topic Mapping](./ss/Screenshot%202026-08-09%20153210.png)

### Managed Topics Dashboard View
Web interface tracking the newly initialized topic matrix, confirming that the new data topic is healthy and reporting active partition counts on the cluster backend.

![Managed Topics Dashboard View](./ss/Screenshot%202026-08-09%20153354.png)

---

## 🚀 Step 4: Security Provisioning & Live Stream Testing

### Generating API Keys & Local Payload Production
Generated fresh cluster API credentials to securely validate connections. After targeting the active key resource, I initialized a live terminal producer to send structured JSON payloads straight into the cloud broker.

![Generating API Keys & Local Payload Production](./ss/Screenshot%202026-08-09%20155336.png)

### Cloud Message Ledger Verification
The Confluent Cloud dashboard capturing incoming timestamps, offsets, and message partitions in real-time, verifying that data successfully left the terminal environment and hit the cloud securely.

![Cloud Message Ledger Verification](./ss/Screenshot%202026-08-09%20155402.png)

### Side-by-Side End-to-End Live Stream Validation
A side-by-side terminal verification test showing decoupled terminal panes operating simultaneously. A terminal producer broadcasts data packets on one side, while an independent console consumer continuously polls the topic to decode and print the streaming data in real-time.

![Side-by-Side End-to-End Live Stream Validation](./ss/Screenshot%202026-08-09%20155943.png)

---
*🔒 **Security Note:** All private API keys, cluster paths, and secrets visible in these screenshots have been fully deleted or deactivated inside the Confluent Cloud dashboard to prevent unauthorized infrastructure usage.*
