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
---

## Docker Verification

Before deploying Kibana, I verified that Docker was installed and available on the Ubuntu virtual machine.

```bash
docker --version
---

## Troubleshooting

During the lab, I encountered an issue when restarting the Kibana container.
I first checked the container status using:
sudo docker ps -a
The Kibana container was still present but had stopped.
When I attempted to restart it, Docker returned an error involving the Elasticsearch certificate path /tmp/http_ca.crt.
I checked the path and discovered that it had become a directory instead of the certificate file expected by the container.
I corrected the certificate path by restoring the Elasticsearch HTTP CA certificate and then restarted Kibana successfully.
After troubleshooting, I verified the container again using:
sudo docker ps
Kibana returned to an Up status with port 5601 mapped correctly.
---

## What I Learned

This troubleshooting process gave me practical experience with Docker container management, certificate paths, bind mounts, port mapping, and using error messages to identify configuration problems.
---

## Current Status

Elasticsearch is installed and running on Ubuntu.
Kibana 9.5.0 ARM64 is deployed through Docker.
The Kibana container is running successfully.
Port 5601 is mapped for Kibana.
Kibana installation, verification, and troubleshooting are documented.
