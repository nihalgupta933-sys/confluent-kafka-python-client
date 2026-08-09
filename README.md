# Confluent Kafka & Python Client Implementation

A comprehensive, hands-on implementation demonstrating real-time message stream management on the cloud. This project highlights cluster interactions utilizing both programmatic Python microservices and automated terminal operations via the command-line interface on Windows.

---

## ☁️ Cloud Infrastructure Notice
Everything in this repository was deployed, hosted, and executed entirely on **Confluent Cloud Kafka**. 

💡 **Free Training Resource:** If you want to replicate this project or explore Kafka on the cloud for free, you can use the promotional coupon code below during your Confluent Cloud signup phase to receive free credits for your first month of usage:
* **Coupon Code:** `CONFLUENTDEV1`

---

## 🛠️ What I Did in Kafka

Through this implementation, I completed the following architectural and engineering tasks:
1. **Cloud Environment Configuration:** Set up and provisioned a secure environment and a dedicated Kafka cluster (`cluster_0`) entirely within the Confluent Cloud ecosystem.
2. **Topic Architecture:** Architected and created specific Kafka topics to store incoming real-time event messages safely.
3. **Programmatic Microservices:** Wrote standalone Python client modules (Producers & Consumers) using SASL_PLAIN secure authentication over SSL protocols.
4. **Live Data Streaming:** Transmitted live text messages into the cloud broker from a Python client and successfully read those streams back out in real-time.
5. **DevOps Terminal Automation:** Installed, configured, and operated the official Confluent CLI tools to audit the cloud environment directly from a Windows PowerShell terminal.

---

## 📁 Repository Directory Structure

Explore the individual components of this project through the links below:

* ### [📁 Python Client](./Python%20Client/)
  Contains the core programmatic implementation files, including the Jupyter Notebook (`.ipynb`) source codes for both the message Producer and Consumer scripts. This directory also contains visual execution screenshots confirming data transmissions.
  
* ### [📁 Terminal (CLI-Execution)](./Terminal(CLI-Execution)/)
  Houses direct, unedited step-by-step terminal execution output screenshots. These verify successful environment audits, authentication checkpoints, and manual topic verification operations performed natively through the command prompt.

* ### [📄 windows-setup-commands.txt](./windows-setup-commands.txt)
  A clean, single-line script reference containing the automated Windows Package Manager (`winget`) installation sequence utilized to seamlessly configure the Confluent CLI binary onto Windows systems.

---
*Security Note: In accordance with enterprise cloud security best practices, all production bootstrap server URLs, API keys, usernames, and passwords have been strictly replaced with generic placeholders in the public source code files.*

