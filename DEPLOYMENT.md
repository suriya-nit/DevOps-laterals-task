# Level 3 – Cloud Deployment

This project is deployed on a cloud virtual machine using Docker and Docker Compose.

## Cloud Environment
- Linux VM (Ubuntu)
- Docker & Docker Compose installed

## Deployment Steps
1. Clone the repository on the cloud VM
2. Navigate to the project root
3. Run:
   docker compose up -d

## Architecture
- Frontend and backend are containerized
- Nginx acts as a reverse proxy
- Application is exposed publicly on port 80

## CI/CD
A Jenkins pipeline is included (Jenkinsfile) for automated builds.
