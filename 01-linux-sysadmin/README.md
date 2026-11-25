# Phase 01: Linux System Administration & Environment Setup

## Objective
Establish a working Ubuntu Linux environment via Windows PowerShell (WSL) to practice system administration, file permissions, network inspection, and system log analysis as the foundation for cloud and security operations.

## Key Activities & Commands
- **System & Resource Inspection:** Checked OS details, disk usage, and running processes (`uname -a`, `df -h`, `top`).
- **Users, Groups & Permissions:** Practiced privilege management and file ownership (`chmod`, `chown`, `sudo`) following the least-privilege mindset.
- **Networking & Ports:** Inspected IP configuration and active listening ports (`ip a`, `ss -tulnp`) and tested connectivity (`ping`, `curl`).
- **Logs Exploration:** Reviewed system and authentication logs under `/var/log` (`auth.log`, `syslog`) to understand how events are recorded.

## Security Takeaway
Understanding Linux permissions, exposed ports, and log files is essential before deploying cloud workloads or monitoring security events.
