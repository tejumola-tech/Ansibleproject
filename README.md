# Ansible Project: Server Automation Tasks

This repository contains simple Ansible playbooks created while learning how to automate server configuration and setup. These tasks are tested on an Amazon Linux 2023 EC2 instance using SSH key-based authentication.

## 📁 Files in this Project

| File Name              | Description |
|------------------------|-------------|
| `inventory.ini`        | Defines the target EC2 host(s) for Ansible to run tasks on. |
| `install-docker.yml`   | Installs Docker on the remote EC2 instance. |
| `install-ngnix.yml`    | Installs and starts NGINX web server on the EC2 instance. |
| `add-user.yml`         | Creates a new user (`deployer`) on the EC2 server and sets up SSH key access. |
| `copy-resume.yml`      | Copies a local `.docx` file (resume) to the EC2 instance. |
| `check-resource.yml`   | Checks memory and CPU usage on the remote EC2 server. |

## 🧪 How to Run a Playbook

Make sure you have:
- Ansible installed
- SSH key available
- Updated `inventory.ini` with the correct IP address or hostname

Example:

```bash
ansible-playbook -i inventory.ini install-docker.yml
