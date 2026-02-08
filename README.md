# Randori EASM by IBM For Splunk App


## Overview

Randori External Attack Surface Management (EASM) by IBM for Splunk provides full visibility into an organization’s externally exposed digital footprint using the Randori EASM APIs.

This Splunk App enables security teams to **discover, monitor, analyze, and operationalize external attack surface data** directly in Splunk—without relying on the Randori External Attack Surface Management (EASM) portal User Interface.

![Python](https://img.shields.io/badge/python-3.10%2B-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Status](https://img.shields.io/badge/status-active%20development-yellow.svg)



---
⚠️ Disclaimer

This Splunk App is not an official Randori EASM by IBM  products or utility.

Use of this software is not covered by any license, warranty, or support agreement you may have with Randori EASM by IBM.


## Key Functions & Features

- **Internet Mapping**: Continuous scanning of public IP addresses and domains to build a detailed, searchable map of internet assets (hosts, services, certificates).
- **Attack Surface Management (ASM)**: Identification of unknown, vulnerable, or misconfigured internet-facing assets to reduce blind spots.
- **Threat Hunting**: Rich datasets and pivots for proactive investigation and detection.
- **Deep Context**: Asset-level metadata including software, TLS, WHOIS, geolocation, and CVE associations.
- **Platform & API Access**: Search engine, REST APIs, and integrations supporting large-scale analytics.

---

## Supported Asset and Intelligence Types

Randori EASM by IBM provides visibility into the following externally observable assets and metadata:

- IP Addresses
- Hosts and Services
- Open Ports and Protocols
- Software and Product Fingerprints
- SSL/TLS Certificates
- Certificate Authorities
- Domains and Hostnames
- Autonomous System Numbers (ASNs)
- Organizations
- Geolocation Metadata
- Internet-Wide Search Results
- EASM Inventory and Discoveries (licensed)

---

## Features

### 🛡️ Core Capabilities

| Feature | Description |
|------|-------------|
| 🌐 External Asset Discovery | Identify exposed hosts and services |
| 🔍 Internet-Wide Search | Query the Cycognito scan index |
| 🧭 Host Intelligence | Deep inspection of services and banners |
| 🧬 Certificate Intelligence | SSL/TLS certificate visibility |
| 🕵️ Exposure Context | Protocols, software, and metadata |
| 🧾 Evidence Preservation | Raw API responses retained |

---

### 📈 Analytics and Visibility

| Feature | Description |
|------|-------------|
| 📊 Exposure Trends | Track asset and service changes |
| 🔄 First-Seen Detection | Identify newly observed assets |
| 🧱 Infrastructure Mapping | IP → ASN → Organization |
| 🔐 Certificate Monitoring | Certificate inventory and metadata |
| 🧠 Investigative Pivoting | Pivot across IPs, domains, certs |

---

### ⚙️ Operational Excellence

| Feature | Description |
|------|-------------|
| 📡 Modular Input Framework | Secure API-based ingestion |
| 🔑 Credential Management | Encrypted credential storage |
| 🌐 Proxy Support | Enterprise proxy compatibility |
| 🩺 Health Monitoring | API reachability and status |
| 📋 Operational Logging | Full ingestion traceability |
| ⏱️ Rate-Limit Awareness | Throttling-safe polling |

---

## 📊 Dashboards

| Dashboard | Description |
|---------|-------------|
| Overview | High-level external exposure summary |
| Hosts | Internet-exposed hosts and services |
| Services | Port, protocol, and software analysis |
| Certificates | SSL/TLS certificate inventory |
| Domains | Domain and hostname visibility |
| ASN Exposure | ASN-level exposure analysis |
| New Assets | Newly observed assets |
| Search Analytics | Search query trends |
| Operations | Ingestion status and metrics |
| Health | API and data freshness monitoring |

Dashboards are designed for **investigation-first workflows**, not executive summaries.

