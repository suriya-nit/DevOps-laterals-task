# DevOps Laterals Task

## Overview
This project demonstrates containerization, reverse proxying, CI/CD pipeline setup,
and cloud deployment using industry-standard DevOps tools.

---

## Architecture
- Frontend: Dockerized web application
- Backend: Dockerized API service
- Nginx: Reverse proxy serving frontend and routing API requests
- Docker Compose: Orchestrates multi-container setup
- Jenkins: CI/CD pipeline for automated builds

---

## Local Setup
1. Clone the repository
2. Navigate to project root
3. Run:
   docker compose up --build
4. Access application at:
   http://localhost

---

## CI/CD Flow (Level 2)
1. Jenkins pulls the latest code from GitHub
2. Jenkins builds Docker images using docker-compose
3. Pipeline stages are defined using Jenkinsfile

Deployment stage is intentionally kept minimal and can be extended to full automation.

---

## Cloud Deployment (Level 3)
The application is deployed on a cloud virtual machine using Docker and Docker Compose.

Steps:
1. Provision a Linux VM
2. Install Docker and Docker Compose
3. Clone repository
4. Run:
   docker compose up -d

The application becomes publicly accessible via the VM’s public IP.

---

## Infrastructure Automation (Optional)
Terraform and Ansible can be added in future to automate infrastructure provisioning
and configuration management.

## Execution Evidence

Due to limited time and system constraints, screenshots and execution logs
are not attached.

However, all required configurations including Dockerfiles, docker-compose.yml,
Nginx reverse proxy configuration, and Jenkinsfile have been provided and verified
locally.

The CI/CD pipeline is defined as a working skeleton and can be executed by
configuring Jenkins credentials and runtime environment.
