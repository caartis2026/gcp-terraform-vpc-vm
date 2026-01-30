# GCP Terraform VPC + VM Deployment

This project demonstrates **production-style infrastructure provisioning on Google Cloud Platform (GCP)** using **Terraform**.

It provisions:
- A custom **VPC network**
- A **subnet** in `us-central1`
- A **firewall rule** allowing SSH
- A **Compute Engine VM** (Debian 12)

This repository is designed to showcase **Infrastructure as Code (IaC)** skills for cloud and data engineering roles.

---

## Architecture Overview

- **Cloud Provider:** Google Cloud Platform
- **Region:** us-central1
- **Zone:** us-central1-a
- **VM Type:** e2-micro (cost-efficient)
- **OS:** Debian 12
- **Networking:**
  - Custom VPC (no auto subnet creation)
  - Custom subnet `10.10.0.0/24`
  - SSH access via firewall rule

---

## Prerequisites

Before running this project, you need:

- A Google Cloud account
- A GCP project with billing enabled
- Terraform installed (`>= 1.x`)
- Google Cloud CLI (`gcloud`)
- Authenticated with:
  ```bash
  gcloud auth application-default login
