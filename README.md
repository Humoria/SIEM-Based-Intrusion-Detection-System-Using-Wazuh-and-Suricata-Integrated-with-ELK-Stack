# SIEM-Based Intrusion Detection System Using Wazuh and Suricata Integrated with ELK Stack

This project demonstrates the implementation of a Security Information and Event Management (SIEM) system by combining **Wazuh**, **Suricata**, and the **ELK Stack** to provide comprehensive intrusion detection capabilities on both the host and network level.

## 📌 Overview

- **Wazuh**: Provides host-based intrusion detection, log analysis, integrity monitoring, and active response.
- **Suricata**: An open-source network threat detection engine for real-time intrusion detection (IDS), intrusion prevention (IPS), and network security monitoring (NSM).
- **ELK Stack** (Elasticsearch, Logstash, Kibana): Serves as a powerful platform for indexing, analyzing, and visualizing logs from both Wazuh and Suricata.

## 🧰 Components Used

| Component    | Description                                 |
|--------------|---------------------------------------------|
| Wazuh        | Host-based security monitoring              |
| Suricata     | Network-based IDS/IPS                       |
| Filebeat     | Log forwarder from Wazuh & Suricata         |
| Logstash     | Parses and processes incoming logs          |
| Elasticsearch| Stores and indexes log data                 |
| Kibana       | Data visualization and dashboarding         |
| Ubuntu 20.04 | Operating System for deployment             |

## ⚙️ System Architecture

The system architecture integrates Wazuh and Suricata on a single Ubuntu server. Both agents forward their logs to the ELK Stack for unified analysis and real-time alerting.

