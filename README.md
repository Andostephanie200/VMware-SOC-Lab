# VMware SOC Home Lab

## Project Overview

This project documents a hands-on cybersecurity home lab built using VMware Fusion on a MacBook Pro.

The lab provides an isolated environment for practicing cybersecurity, system administration, network analysis, and SOC (Security Operations Center) monitoring skills.

The environment includes multiple virtual machines and security tools that allow me to safely practice security monitoring and investigation techniques without affecting my primary operating system.

---

## Project Goal

The goal of this project is to build and document a practical SOC-style environment where I can develop hands-on skills in:

* Security monitoring
* Log analysis
* Network traffic analysis
* SIEM concepts
* Incident investigation
* Linux administration
* Windows security monitoring
* Virtualization
* Cybersecurity troubleshooting

---

## Lab Environment

The lab is hosted using VMware Fusion and includes the following virtual machines:

* **Windows 11** — Windows endpoint used for security monitoring and testing
* **Ubuntu Linux** — Linux environment hosting security monitoring components
* **Kali Linux** — Security testing and analysis environment

### Security Tools

* **Elasticsearch** — Used to store, search, and analyze security-related data and logs
* **Wireshark** — Used for network traffic capture and packet analysis
* **VMware Fusion** — Used to create and manage the virtualized lab environment

---

## Architecture

The lab architecture connects the virtual machines and security tools into a controlled environment for cybersecurity practice.

The architecture diagram can be found in the **Diagram** folder.

---

## Elasticsearch

Elasticsearch was installed on the Ubuntu virtual machine as part of the lab's security monitoring environment.

### Installation and Verification

The Elasticsearch installation was verified by:

1. Checking the Elasticsearch system service.
2. Confirming that the service was **active (running)**.
3. Testing the Elasticsearch API through the local HTTPS endpoint.
4. Authenticating using the Elasticsearch `elastic` account.
5. Confirming that Elasticsearch returned cluster and version information.

### Evidence

Screenshots documenting the Elasticsearch installation and verification process are available in the **screenshots** folder.

---

## Wireshark

Wireshark is used in this lab for network traffic analysis and packet inspection.

It provides hands-on practice with:

* Packet capture
* Protocol analysis
* Network troubleshooting
* Identifying unusual network activity
* Understanding network communications

---

## Skills Developed

Through building and troubleshooting this lab, I have developed hands-on experience with:

* VMware virtualization
* Windows administration
* Linux administration
* Elasticsearch
* Network traffic analysis
* Wireshark
* Security monitoring concepts
* Log analysis
* Troubleshooting
* SOC environment design
* Technical documentation

---

## Project Documentation

Additional documentation, diagrams, and screenshots are available in the repository:

* **Diagram** — Lab architecture
* **Note** — Project notes and technical documentation
* **Screenshots** — Evidence from the lab setup and configuration

---

## Current Project Status

### Completed

* VMware Fusion lab environment
* Windows 11 virtual machine
* Ubuntu Linux virtual machine
* Kali Linux virtual machine
* Wireshark setup
* Elasticsearch installation
* Elasticsearch service verification
* Elasticsearch API verification
* GitHub project documentation

### In Progress

* Kibana setup
* Security monitoring workflow
* Log collection and analysis
* SOC investigation exercises

---

## Disclaimer

This project is a controlled home laboratory created for educational and cybersecurity skill-development purposes.
