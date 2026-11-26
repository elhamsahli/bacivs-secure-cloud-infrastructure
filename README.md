# BACIVS — Secure Cloud Infrastructure (DevSecOps Portfolio)

A hands-on DevSecOps infrastructure project demonstrating the progression from a hardened local container environment (**Windows 11 + WSL 2 + Docker**) to a segmented, production-grade cloud architecture on **Oracle Cloud Infrastructure (OCI)**.

---

## Architecture & Methodology

This repository follows a **document-after-doing** approach—every architectural decision, configuration, and security control is implemented and verified before being documented:

1. **Local Foundation:** Hardened Linux administration and non-root Docker container workflows on WSL 2 (Ubuntu).
2. **Cloud Networking (OCI):** Isolated Virtual Cloud Network (VCN) with public/private subnets and strict Security Lists.
3. **Compute & Container Deployment:** Secure compute provisioning, hardened container workloads, and automated CI/CD checks.

---

## Project Phases & Repository Structure

| Phase | Module / Directory | Focus Area | Status |
| :--- | :--- | :--- | :--- |
| **Phase 01** | [`01-linux-sysadmin`](./01-linux-sysadmin/README.md) | Linux System Administration, Least-Privilege Permissions, & Local Container Environment (WSL 2 & Docker) | Completed |
| **Phase 02** | `02-oci-network-vcn` | Oracle Cloud VCN Architecture, Public/Private Subnets, Gateways, & Security Lists | In Progress |
| **Phase 03** | `03-secure-compute-containers` | Hardened OCI Compute Instance, Custom Dockerfile, & Read-Only Container Deployment | Planned |
| **Phase 04** | `04-devsecops-automation` | Infrastructure as Code (Terraform), Vulnerability Scanning, & CI/CD Security Gates | Planned |

---

## Key Security Controls Implemented

- **Least-Privilege Access:** Enforced strict Linux file permissions (`chmod`/`chown`) and non-root container execution via the `docker` group.
- **Immutable Container Mounts:** Mounted host volumes as read-only (`:ro`) to prevent runtime tampering.
- **Network Segmentation *(Upcoming)*:** Isolating backend services inside private OCI subnets with minimal ingress rules.
