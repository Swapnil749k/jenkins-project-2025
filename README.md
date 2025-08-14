# Jenkins Project: Swiggy Clone App Deployment
🍔 Swiggy Clone App Deployment – DevOps Project
📌 Project Overview

This project demonstrates the end-to-end CI/CD pipeline for deploying a Swiggy Clone Application using modern DevOps practices and tools.
The goal is to ensure automated provisioning, code quality checks, vulnerability scanning, containerization, and cloud deployment using:

Terraform → Infrastructure as Code

AWS → Cloud hosting & services

Jenkins → CI/CD pipeline orchestration

GitHub → Source code & version control

SonarQube → Static code analysis & quality gates

Trivy → Container image vulnerability scanning

Docker → Containerization & image management

🚀 Tools & Technologies Used
Tool/Service	Purpose
Terraform	Provision AWS resources (EC2, S3, EKS, etc.)
AWS	Cloud infrastructure & application hosting
Jenkins	Automating build, test, scan, and deployment
GitHub	Source code management
SonarQube	Code quality & bug detection
Trivy	Security scanning for Docker images
Docker	Packaging and shipping the application
🛠️ Architecture Workflow

Developer commits code to GitHub.

Jenkins Pipeline is triggered automatically.

SonarQube Analysis checks code quality.

Trivy Scan detects vulnerabilities in Docker images.

Terraform provisions AWS infrastructure.

Docker builds and pushes the image to ECR/DockerHub.

Application deployed to AWS (EC2 / EKS / ECS).

📂 Project Structure
swiggy-clone-deployment/
│
├── terraform/               # IaC scripts for AWS
├── jenkins/                 # Jenkins pipeline configuration
├── src/                     # Application source code
├── Dockerfile                # Docker build instructions
├── sonar-project.properties  # SonarQube configuration
├── README.md                 # Project documentation

📋 Prerequisites

AWS account with required IAM permissions

Jenkins server with required plugins:

SonarQube Scanner

Docker Pipeline

Terraform

SonarQube server configured

Docker & Trivy installed

GitHub repository access

⚙️ Steps to Deploy

Clone the Repository

git clone https://github.com/your-username/swiggy-clone-deployment.git
cd swiggy-clone-deployment


Configure Terraform with AWS credentials.

Setup Jenkins Pipeline using Jenkinsfile.

Run the Pipeline to:

Analyze code (SonarQube)

Scan vulnerabilities (Trivy)

Build & push Docker image

Deploy to AWS infrastructure

✅ Key Features

Automated Infrastructure provisioning with Terraform

Code quality gates with SonarQube

Security-first approach with Trivy

Continuous Integration & Deployment with Jenkins

Scalable & containerized deployment using Docker & AWS.
