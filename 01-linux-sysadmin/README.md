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
### Local Container Environment (WSL 2 & Docker)

Configured a local container runtime on **Windows 11** using **WSL 2 (Ubuntu)** integrated with **Docker Desktop** as the initial foundation before transitioning to **Oracle Cloud Infrastructure (OCI)**:

- **WSL 2 & Docker Desktop Integration:** Enabled WSL 2 integration for Ubuntu in Docker Desktop and verified daemon connectivity from the Ubuntu terminal.
- **Socket Permissions & Session Handling:** Added the Linux user to the `docker` group (`sudo usermod -aG docker $USER`) and restarted the WSL session (`wsl --shutdown`) so Docker CLI commands run without `sudo`.
- **Container Verification & Volume Mounting:** Validated runtime functionality with `hello-world`, then deployed an `nginx:alpine` test container (`-p 8080:80`) with a local host directory (`~/bacivs-web`) mounted read-only (`:ro`) to `/usr/share/nginx/html` and verified HTTP responses via `curl`.
