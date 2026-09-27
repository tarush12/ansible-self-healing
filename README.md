# AWS Ansible Configuration Drift Detection & Automated Remediation

## Overview

This project uses Ansible to manage an Ubuntu EC2 instance on AWS and maintain the desired Nginx configuration.

The project demonstrates configuration management, health checks, configuration drift detection, and automated remediation.

## Architecture

WSL Ubuntu
(Ansible Control Node)
        |
        | SSH
        |
        v
AWS EC2 Ubuntu
(Managed Node)
        |
        v
Nginx

## Technologies Used

- AWS EC2
- Ansible
- Linux / Ubuntu
- SSH
- Nginx
- YAML
- Git / GitHub

## Project Structure

```text
ansible-self-healing/
├── ansible.cfg
├── inventory/
│   └── hosts.ini.example
├── playbooks/
│   └── site.yml
├── roles/
│   ├── nginx/
│   └── health_check/
├── nginx.conf.j2
├── .gitignore
└── README.md
