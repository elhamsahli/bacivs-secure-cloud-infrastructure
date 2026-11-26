# Phase 02: Oracle Cloud Infrastructure (OCI) — Secure VCN Architecture

## Objective
Design and deploy an isolated, segmented Virtual Cloud Network (VCN) on Oracle Cloud Infrastructure following least-privilege network security principles.

## Planned Architecture
- **VCN CIDR Block:** `10.0.0.0/16`
- **Public Subnet (`10.0.1.0/24`):** Hosts bastion/ingress resources with controlled Internet Gateway access.
- **Private Subnet (`10.0.2.0/24`):** Isolates backend workloads and containers with NAT Gateway outbound-only access.
- **Security Lists:** Strict stateful ingress/egress rules restricting SSH (`22`) and HTTP/HTTPS (`80`/`443`).

## Status
- [ ] Create VCN & Subnets
- [ ] Configure Internet & NAT Gateways
- [ ] Harden Security Lists & Route Tables
- [ ] Document Architecture & Verification
