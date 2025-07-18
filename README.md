# Splunk + Wazuh + Elastic Stack Integration Guide

This repository documents the integration of Splunk Enterprise with the Wazuh security platform and the Elastic Stack to create a hybrid visibility and detection architecture. This setup enables real-time monitoring of Windows event logs, advanced rule-based alerting, and correlation with MITRE ATT&CK tactics.

---

## Why Familiarity with Splunk is Important

Splunk is a widely adopted platform in enterprise environments for log aggregation, threat detection, and security analytics. Familiarity with Splunk is essential for any SOC analyst or security engineer because it provides:

- Centralized log collection and real-time event analysis
- The ability to search and query data using SPL (Search Processing Language)
- Support for alerting, dashboards, and reports used in day-to-day SOC operations
- Integration with ticketing systems, automation tools, and threat intelligence platforms

Understanding how to ingest data, create custom alerts, and respond to incidents using Splunk is critical for effective monitoring, triage, and threat detection.

---

## Advantages of Integrating Splunk with Wazuh and the Elastic Stack

Integrating Splunk with Wazuh and the Elastic Stack combines the strengths of each platform to build a layered detection strategy:

### 1. Layered Detection

- Splunk enables log search, dashboarding, and alert creation
- Wazuh adds rule-based correlation and alert enrichment
- Elastic Stack provides scalable storage and query capabilities through Elasticsearch and Kibana

### 2. Threat Intelligence and MITRE Mapping

- Wazuh maps alerts to MITRE ATT&CK techniques out of the box
- Security teams can identify and investigate tactics and behaviors based on real-world frameworks

### 3. Enhanced Visualization and Alerting

- Splunk can be used for real-time visual dashboards and Tier 1 visibility
- Kibana with the Wazuh plugin supports historical analysis, custom visualizations, and attack timelines

### 4. Cost-Effective and Scalable Architecture

- Wazuh is open-source and lightweight
- Splunk can be selectively used to monitor premium or high-priority data sources
- Ideal for hybrid SOC labs or production environments with budget constraints

### 5. Red Team vs Blue Team Lab Simulation

- Wazuh agents and Splunk forwarders allow testing of adversarial behavior
- Enables log capture from both red team attack simulations and defensive detections
- Supports the development of custom rules, alerts, and correlation strategies

---

## Use Cases

- Monitoring Windows Event Logs (4624, 4625, 4672, etc.)
- Detecting privilege escalation, account creation, or service installation
- Visualizing brute force attempts and successful logons
- MITRE ATT&CK technique mapping for incident response and reporting
- Dual-platform alerting with Splunk saved searches and Wazuh rules

---

## Summary

Combining Splunk with Wazuh and the Elastic Stack provides an enterprise-grade monitoring solution that balances real-time searchability with contextual detection. It enhances visibility across endpoints, supports attack simulation and defense workflows, and builds a resilient foundation for security operations.

