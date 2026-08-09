# 🐍 Python Client & Cloud Monitoring

This directory tracks my hands-on experience using Python to programmatically interface with Confluent Cloud Kafka. By separating the transmission logic into distinct files, I simulated a real-world asynchronous system where a publisher can broadcast streams completely independent of the listener.

---

## 🏗️ Phase 1: Baseline Verification (Cloud UI Tests)
Before testing custom Python automation, I used the native Confluent Cloud interface to verify that my backend topic infrastructure was active and accepting data.

### Initial Smoke Test
Manually published a dummy test message inside the Confluent UI dashboard. This verified that partition configurations, keys, and values (`0`) were routing accurately through the cloud cluster.

![Initial Smoke Test](./ss/Screenshot%202026-08-07%20203036.png)

---

## 🚀 Phase 2: Programmatic Event Production

### 📁 Core Script: [Confluent-Kafka Producer.ipynb](./Confluent-Kafka%20Producer.ipynb)
This interactive notebook configures the core operational settings required to authenticate safely with Confluent Cloud. It uses standard `confluent-kafka` client libraries over a secure SSL channel to stream simulated data payloads.

### Stream Lineage Overview
Illustrates the macro-level event data flow mapping. It displays the connection coming directly from my custom Python producer client routing straight into the active `ecommerce` cloud topic on AWS (`us-east-2`).

![Stream Lineage Overview](./ss/Screenshot%202026-08-08%20133719.png)

### Live Cloud Message Inspection
Verifies successful JSON serialization of data payloads. The cloud console captures the raw text parameters confirming structured message attributes are passing correctly into the cloud environment.

![Live Cloud Message Inspection](./ss/Screenshot%202026-08-08%20133800.png)

### High-Volume Traffic Monitoring
Captures a live throughput spike graph processing an extended sequence of 248 messages within a brief sampling period, proving the pipeline can handle continuous real-time loads.

![High-Volume Traffic Monitoring](./ss/Screenshot%202026-08-08%20143445.png)

---

## 📥 Phase 3: Continuous Event Consumption

### 📁 Core Script: [Confluent-Kafka Consumer.ipynb](./Confluent-Kafka%20Consumer.ipynb)
This module acts as the downstream consumer system. It utilizes an infinite polling loop (`while True`) to pull, decode, parse, and verify active string message packets streaming directly off the cloud brokers.

### Consumer Lineage Visualizer
Displays the updated cluster mapping showing the data stream successfully exit the `ecommerce` topic bucket and land smoothly inside my localized application consumer group layout (`customer_grp`).

![Consumer Lineage Visualizer](./ss/Screenshot%202026-08-08%20194624.png)

### Total Message Auditing
Confirms the cumulative storage volume checkpoint inside the cloud backend, logging a final index count of exactly 249 verified string rows maintained safely on the cluster.

![Total Message Auditing](./ss/Screenshot%202026-08-08%20194704.png)

### Local Console Output Capture
A direct snapshot of the Google Colab terminal processing live data. It displays the parsed output log tracking streaming message data alongside standard error-handling exceptions.

![Local Console Output Capture](./ss/Screenshot%202026-08-08%20200734.png)

### End-to-End Value Synchronization
Concludes the verification by comparing side-by-side execution frames. It shows my local Python console capturing unique testing strings (like `{'value': 'Aldrago'}`) at the exact moment they sync with the matching payload indexes inside the Confluent web debugger console.

![End-to-End Value Synchronization](./ss/Screenshot%202026-08-09%20142400.png)

---
*🔒 **Security Note:** To maintain profile privacy, all live cluster server hostnames, secret keys, usernames, and passwords have been entirely replaced with dummy placeholder configuration values across both notebook files.*
