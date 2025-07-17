🛠️ End-to-End DevOps Implementation for Open-Source E-Commerce Application

This repository documents a complete DevOps implementation for an open-source e-commerce application built with multiple microservices. The focus is on deploying the application on AWS using containerization, orchestration, infrastructure-as-code, and automated CI/CD pipelines.

⚠️ Note: This project uses an open-source e-commerce codebase as the application layer. This repository focuses entirely on the DevOps infrastructure and automation built around it.

⸻

🔧 Tech Stack

🧰 Tools & Platforms
	•	Cloud: AWS (EC2, EKS, IAM, VPC, Route 53)
	•	IaC: Terraform
	•	Containerization: Docker, Docker Compose
	•	Orchestration: Kubernetes (EKS)
	•	CI/CD: GitHub Actions, Argo CD
	•	GitOps: Argo CD
	•	Networking: Ingress Controller, Route 53
	•	Source Control: Git, GitHub

⸻

📂 Project Structure Overview

1️⃣ Infrastructure Setup
	•	AWS account setup and IAM role configuration
	•	EC2 instance provisioning
	•	VPC creation and subnet configurations
	•	Security groups and inbound rule setup
	•	Terraform backend and state management

2️⃣ Local Development
	•	Docker installation and configuration
	•	Docker Compose setup for local multi-container testing
	•	Containerization of all microservices
	•	Local test runs of the full app

3️⃣ Terraform Automation
	•	Terraform lifecycle (init, plan, apply, destroy)
	•	VPC and EKS provisioning using Terraform
	•	Terraform state locking and remote backend setup
	•	Terraform modules for reusable infrastructure components

4️⃣ Kubernetes on AWS (EKS)
	•	Configure kubectl for the EKS cluster
	•	Kubernetes manifests: Deployments, Services, Ingress, Storage
	•	Ingress controller setup using Helm
	•	Storage class, PersistentVolume (PV), and PersistentVolumeClaim (PVC)
	•	Deployment and verification of all microservices on EKS

5️⃣ Custom Domain & Networking
	•	Domain setup with Route 53
	•	Subdomain routing to Kubernetes ingress
	•	Secure DNS integration with the EKS cluster

6️⃣ GitOps with Argo CD
	•	Install and configure Argo CD on the EKS cluster
	•	Connect GitHub repo to Argo CD for continuous deployment
	•	Deploy application through GitOps workflow

7️⃣ CI/CD Automation
	•	GitHub Actions workflows for building and pushing Docker images
	•	CI pipeline for microservices
	•	Integration of CI pipeline with Argo CD for automated CD

⸻

✅ Prerequisites
	•	Basic knowledge of DevOps tools and concepts
	•	An active AWS account
	•	Familiarity with Git, Docker, and basic Kubernetes

⸻

🧭 Getting Started

Detailed setup steps coming soon

	1.	Clone this repository:

git clone https://github.com/your-username/devops-ecommerce-project.git
cd devops-ecommerce-project


	2.	Set up AWS credentials
	3.	Run Terraform to provision infrastructure
	4.	Deploy containers and Kubernetes services
	5.	Set up CI/CD with GitHub Actions and Argo CD
	6.	Access application via Route 53 domain and Ingress controller

⸻

📄 Credits

This project uses the following open-source application as the base e-commerce app:
🔗 [Link to original open-source project]

All DevOps scripts, infrastructure, and CI/CD configurations are custom and maintained in this repository.

⸻

📌 License

This project is licensed under the MIT License.
The original open-source application retains its respective license.

⸻
