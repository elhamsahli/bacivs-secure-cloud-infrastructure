# BACIVS — Secure Cloud Infrastructure & DevSecOps Lab

## Project Overview
An end-to-end enterprise infrastructure simulation built around my graduation project (**BACIVS** — Blockchain Academic Certificate Verification System). Rather than treating the application in isolation, this lab demonstrates how to architect, deploy, harden, monitor, and security-test a realistic environment across Linux, Cloud, and Containers.

## Architecture & Tech Stack
- **Application Layer:** FastAPI (Backend) & React.js (Frontend) — *BACIVS*
- **Operating System:** Ubuntu Linux (WSL & Cloud Compute)
- **Cloud Infrastructure:** Oracle Cloud Infrastructure (OCI — VCN, Subnets, Security Lists)
- **Containerization:** Docker & Docker Compose
- **Security & Monitoring:** SSH Key Hardening, Linux Firewall (UFW), Log Analysis / Wazuh SIEM
- **Security Testing:** Authorized Vulnerability & Port Auditing (Nmap, API Security Checks)

## Project Roadmap
- [x] **Phase 1:** Linux System Administration & Environment Setup (`01-linux-sysadmin/`)
- [ ] **Phase 2:** Cloud Infrastructure & Network Architecture on OCI (`02-oci-cloud-networking/`)
- [ ] **Phase 3:** Containerizing BACIVS with Docker (`03-docker-deployment/`)
- [ ] **Phase 4:** Infrastructure & Container Security Hardening (`04-security-hardening/`)
- [ ] **Phase 5:** Centralized Logging & SIEM Monitoring (`05-siem-monitoring/`)
- [ ] **Phase 6:** Authorized Security Testing & Remediation Report (`06-security-testing-report/`)
