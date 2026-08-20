# Kibana Installation and Configuration

## Overview

As part of my VMware SOC Home Lab, I deployed Kibana to provide a visual interface for working with Elasticsearch and to continue building a security monitoring and log-analysis environment.

Because my lab runs on an ARM-based environment, I used Docker to deploy an ARM64-compatible Kibana image.

This documentation records the installation, container deployment, verification, and troubleshooting steps performed during the lab.

---

## Lab Environment

### Host System

- MacBook Pro with Apple Silicon
- VMware Fusion

### Ubuntu Virtual Machine

- Ubuntu Linux
- ARM64 / AArch64 architecture
- Elasticsearch 9.5.0
- Docker

### Security Tools

- Elasticsearch
- Kibana
- Wireshark

---

## Why Kibana?

Kibana provides a graphical interface for exploring and visualizing data stored in Elasticsearch.

In a SOC environment, tools such as Kibana can help analysts:

- Search and analyze security logs
- Investigate security events
- Visualize security-related data
- Monitor activity across systems
- Build dashboards for security monitoring

For this home lab, Kibana is being added as the visualization and analysis layer for the Elasticsearch environment.

---

## Architecture Consideration

My MacBook Pro uses Apple Silicon, and the Ubuntu virtual machine runs on ARM64 architecture.

I verified the Ubuntu architecture using:

```bash
uname -m
