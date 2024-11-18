# End-to-End Kubernetes Three-Tier DevSecOps Project

This project demonstrates an end-to-end **Kubernetes Three-Tier Architecture** with integrated **DevSecOps practices**, including CI/CD pipelines, security scans, and monitoring. The architecture uses a **Frontend, Backend, and Database Tier** with all layers secured and automated.

## **Key Features**
- **CI/CD Integration**:
  - Automated pipelines with Jenkins for Continuous Integration and Deployment.
  - Secure Docker image scanning using Trivy.
  - Deployment file updates and artifact storage in a private ECR repository.

- **DevSecOps Practices**:
  - Code quality analysis and dependency checks.
  - Kubernetes monitoring using tools like Prometheus and Grafana.
  - Secrets management using Kubernetes Secrets for ECR and databases.

- **Three-Tier Architecture**:
  - **Frontend Tier**: Managed as pods with Kubernetes Service for load balancing.
  - **Backend Tier**: Interacts with the database and is designed for scalability.
  - **Database Tier**: Uses Persistent Volumes (PVs) for secure and persistent data storage.

- **Infrastructure as Code (IaC)**:
  - Terraform used to provision cloud infrastructure.
  - ArgoCD for GitOps-based continuous deployment.

## **Architecture Overview**
![Architecture Diagram](https://github.com/umarlhepk/End-to-End-Kubernetes-Three-Tier-DevSecOps-Project/blob/main/Three-Tier.gif)

## **Tech Stack**
- **CI/CD Tools**: Jenkins, ArgoCD, GitHub Actions
- **Infrastructure**: Kubernetes, AWS EKS, Terraform
- **Security Tools**: Trivy, ECR Scanning
- **Monitoring**: Prometheus, Grafana
- **Others**: GoDaddy for DNS, ALB for load balancing
