# Elasticsearch Installation and Verification

## Overview

As part of my VMware SOC Home Lab, I installed and configured Elasticsearch on an Ubuntu Linux virtual machine.

The purpose of adding Elasticsearch to the lab is to build hands-on experience with security data storage, searching, and analysis as part of a SOC-style monitoring environment.

This documentation records the installation, configuration, verification, and troubleshooting steps performed during the lab.

---

## Lab Environment

### Host System

- MacBook Pro
- VMware Fusion

### Virtual Machines

- Windows 11
- Ubuntu Linux
- Kali Linux

### Security Tools

- Elasticsearch
- Wireshark

Elasticsearch was installed on the Ubuntu virtual machine.

---

## Why Elasticsearch?

Elasticsearch is a search and analytics engine that can be used to store, search, and analyze large amounts of data.

For this lab, Elasticsearch provides a foundation for building a security monitoring and log-analysis environment.

It is used alongside Kibana to provide a visual interface for exploring and analyzing security-related data within the lab environment.

---

## Elasticsearch Installation

Elasticsearch was installed on the Ubuntu virtual machine.

During the installation process, I encountered compatibility and configuration challenges related to the ARM-based virtual environment.

After troubleshooting the installation and configuration, Elasticsearch was successfully installed and started as a system service.

---

## Service Verification

After installation, I verified that the Elasticsearch service was running using:

```bash
sudo systemctl status elasticsearch
