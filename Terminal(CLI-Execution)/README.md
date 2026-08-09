# 💻 Confluent CLI Terminal Execution Log

This directory archives my practical hands-on experience using the command-line interface (CLI) to configure and operate **Confluent Cloud Kafka** directly from a Windows PowerShell terminal. 

These 10 execution checkpoints showcase a complete administrative lifecycle: authenticating, creating environments/clusters, provisioning API security, and executing live terminal-to-terminal data streaming loops.

---

## 🔐 Step 1: Authentication & Cluster Discovery

### Cloud Login Checkpoint
Initiated connection using the `--save` parameter to authenticate the session securely via my browser environment. The terminal verifies active trial credits ($400+ remaining) and details organic billing safeguards.

![Cloud Login Checkpoint](./ss/Screenshot%202026-08-09%20151117.png)

### Automated Environment Provisioning
Created a dedicated resource sandbox environment named `environment_from_cli`. The system log prints the unique environment metadata (`env-66jv7j`) along with active Essentials data governance packages.

![Automated Environment Provisioning](./ss/Screenshot%202026-08-09%20151837.png)

---

## ☁️ Step 2: Infrastructure Deployment via CLI

### Cloud Console Synchronization
A verified visual checkpoint inside the Confluent Web UI showing my fresh workspace configurations updating instantly on the cloud. The platform lists my original default profile alongside the new `environment_from_cli` bucket.

![Cloud Console Synchronization](./ss/Screenshot%202026-08-09%20152024.png)

### Provisioning a Managed Kafka Cluster
Executed an infrastructure deployment command to spin up a live basic Kafka cluster named `cli_cluster` on AWS (`us-east-1`). The deployment configurations detail storage specs (5000 GB) and security protocol endpoints.

![Provisioning a Managed Kafka Cluster](./ss/Screenshot%202026-08-09%20152338.png)

### Live Cluster Status Audit
A web dashboard checkpoint verifying that `cli_cluster` has successfully finished its deployment cycles and is officially `Running` on the cloud infrastructure.

![Live Cluster Status Audit](./ss/Screenshot%202026-08-09%20152419.png)

---

## 🛠️ Step 3: Topic Design & Security Credentialing

### Resource Selection & Topic Mapping
Targeted my newly active cluster (`lkc-mvk8vg7`) and initialized a fresh data topic named `customer_transaction` with a custom replication factor and 2 distinct logging partitions.

![Resource Selection & Topic Mapping](./ss/Screenshot%202026-08-09%20153210.png)

### Managed Topics Dashboard View
Web view tracking the newly initialized topic matrix, confirming that `customer_transaction` is active with exactly 2 healthy partitions.

![Managed Topics Dashboard View](./ss/Screenshot%202026-08-09%20153354.png)

---

## 🚀 Step 4: Security Provisioning & Live Stream Testing

### Generating API Keys & Local Payload Production
Generated fresh cluster API credentials to securely validate connections. After selecting the key, I initialized a live terminal producer to send JSON string messages (`{"key":123, "value":"hello"}` and `{"key":2006, "value":"I am Aldrago"}`) straight into the cloud broker.

![Generating API Keys & Local Payload Production](./ss/Screenshot%202026-08-09%20155336.png)

### Cloud Message Ledger Verification
The Confluent Cloud dashboard capturing the exact incoming timestamps, offsets, partitions, and message payload values in real-time, verifying that data successfully left the terminal and hit the cloud safely.

![Cloud Message Ledger Verification](./ss/Screenshot%202026-08-09%20155402.png)

### Side-by-Side End-to-End Live Stream Validation
A side-by-side terminal verification test showing independent terminal panes. On the right, a terminal producer broadcasts data packets, while on the left, an independent console consumer polls the topic to decode and print the incoming string payloads natively in real-time.

![Side-by-Side End-to-End Live Stream Validation](./ss/Screenshot%202026-08-09%20155943.png)

---
*🔒 **Security Note:** All private API keys, cluster paths, and secrets visible in these screenshots have been fully deleted or deactivated inside the Confluent Cloud dashboard to prevent unauthorized infrastructure usage.*

