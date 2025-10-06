# Ansible Ubuntu Server Setup

Production-ready Ansible playbooks for automated Ubuntu server configuration and deployment.

## Overview

This repository contains Ansible playbooks and roles used to automate the deployment and configuration of Ubuntu servers in production environments. These playbooks follow best practices for idempotent infrastructure management.

## Features

- **Automated Server Provisioning**: Complete server setup from base Ubuntu installation
- **Security Hardening**: SSH configuration, firewall rules, fail2ban setup
- **Service Deployment**: Automated installation and configuration of common services
- **Idempotent Operations**: Safe to run multiple times without side effects
- **Modular Design**: Reusable roles for different service components

## Playbooks

### `server-baseline.yml`
Initial server configuration including:
- System updates and security patches
- User management and SSH key deployment
- Timezone and locale configuration
- Basic monitoring tools installation

### `web-server.yml`
Web server stack deployment:
- Nginx installation and configuration
- SSL certificate management
- Virtual host setup
- Performance optimization

### `database-server.yml`
Database server configuration:
- PostgreSQL/MySQL installation
- Security configuration
- Backup automation
- Performance tuning

## Requirements
```yaml
ansible: ">=2.9"
python: ">=3.6"
target_os: "Ubuntu 20.04 LTS or newer"