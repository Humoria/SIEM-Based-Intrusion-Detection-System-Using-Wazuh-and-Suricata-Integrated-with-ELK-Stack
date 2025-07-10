# SIEM-Based Intrusion Detection System Using Wazuh and Suricata Integrated with ELK Stack

This project demonstrates the implementation of a Security Information and Event Management (SIEM) system by combining **Wazuh**, **Suricata**, and the **ELK Stack** to provide comprehensive intrusion detection capabilities on both the host and network level.

## 📌 Overview

- **Wazuh**: Provides host-based intrusion detection, log analysis, file integrity monitoring, and active response.
- **Suricata**: An open-source network threat detection engine for real-time intrusion detection (IDS), intrusion prevention (IPS), and network security monitoring (NSM).
- **ELK Stack** (Elasticsearch, Logstash, Kibana): Acts as a centralized platform to collect, index, analyze, and visualize logs from both Wazuh and Suricata.

## 🧰 Components Used

| Component     | Description                                 |
|---------------|---------------------------------------------|
| Wazuh         | Host-based security monitoring              |
| Suricata      | Network-based IDS/IPS                       |
| Filebeat      | Log shipper to ELK Stack                    |
| Logstash      | Log processor for filtering and parsing     |
| Elasticsearch | Stores and indexes log data                 |
| Kibana        | Visualization and dashboard tool            |
| Ubuntu 20.04  | Operating system used for deployment        |

## ⚙️ System Architecture

The architecture integrates Wazuh and Suricata on a single Ubuntu server. Both tools send security logs to the ELK Stack for correlation, alerting, and visualization.

> *(Insert a system topology diagram here, e.g., `system-topology.png` if available)*

## 🚨 Use Cases

- Detect brute-force login attempts
- Identify and analyze suspicious network traffic
- Monitor file system changes on endpoints
- Centralized real-time alerting and visualization

## 🛠️ Installation & Setup

> ⚠️ This setup assumes a clean installation of Ubuntu 20.04.

### 1. Clone this repository

```bash
git clone https://github.com/your-username/wazuh-suricata-siem.git
cd wazuh-suricata-siem
