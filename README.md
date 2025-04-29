# DevOps-mini-project

Complete DevOps CI/CD Mini Project using AWS, Terraform, Jenkins, Docker, Ansible, Kubernetes



## Project Overview

This project demonstrates an end-to-end DevOps CI/CD pipeline integrating major tools and platforms:

- **AWS EC2**: Cloud infrastructure
- **Terraform**: Infrastructure provisioning (IaC)
- **Jenkins**: Continuous Integration / Deployment
- **Docker**: Containerization
- **Ansible**: Configuration management
- **Kubernetes**: Application orchestration

---

## Project Workflow

1. **Terraform** provisions an EC2 instance on AWS.
2. **Jenkins** automates the CI/CD process.
3. **Docker** builds application containers.
4. **Ansible** installs and configures NGINX inside EC2.
5. **Kubernetes** deploys NGINX with a LoadBalancer service.

---

## Technologies Used

| Tool         | Purpose                              |
|--------------|--------------------------------------|
| AWS EC2      | Cloud server hosting                 |
| Terraform    | Provisioning infrastructure          |
| Jenkins      | CI/CD pipeline orchestration         |
| Docker       | Application containerization         |
| Ansible      | Automating server configuration      |
| Kubernetes   | Orchestrating container deployment   |
| Git & GitHub | Source code version control          |

---

## Prerequisites

- AWS account & IAM credentials
- Terraform installed
- Docker & Ansible installed
- Jenkins server setup
- Kubernetes cluster (Minikube or EKS)

---

## Project Files

- `main.tf` – Terraform script to launch EC2
- `Dockerfile` – Creates base image with Ansible & dependencies
- `playbook.yml` – Ansible playbook to install and start NGINX
- `Jenkinsfile` – Jenkins pipeline definition
- `deployment.yaml` – Kubernetes manifest for NGINX deployment
- `ansible.cfg` – Ansible config for localhost
- `README.md` – Project documentation

---

## Usage

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/devops-mini-project.git
cd devops-mini-project