# 🚀 Production-Grade GitOps Microservices Platform on AWS EKS

## 📌 Overview

This project demonstrates a real-world DevOps implementation of a microservices-based e-commerce application deployed on AWS using a GitOps approach.

It simulates a production-grade environment by integrating CI/CD pipelines, containerization, Kubernetes orchestration, and automated deployment using ArgoCD.

---

## 🏗️ Architecture

![Architecture](docs/images/Gitops_Project.png)

The platform follows a modern DevOps workflow:

**Developer → GitHub → CI/CD Pipeline → Docker → Container Registry (ECR) → ArgoCD → AWS EKS → Monitoring**

---

## 🧩 Microservices Architecture

The application is built using a microservices architecture where each service handles a specific business function.

### Core Services:

* Product Catalog Service
* Cart Service
* Payment Service
* Order / Checkout Service
* Shipping Service
* Frontend Service

Each service runs independently and communicates via APIs, enabling scalability and fault isolation.

---

## ⚙️ Tech Stack

* **Cloud**: AWS (EKS, ECR, EC2)
* **Containerization**: Docker
* **Orchestration**: Kubernetes
* **CI/CD**: GitHub Actions / Jenkins
* **GitOps**: ArgoCD
* **Infrastructure as Code**: Terraform
* **Monitoring**: Prometheus, Grafana

---

## 🔥 Key Features

* End-to-end CI/CD pipeline for microservices
* GitOps-based continuous deployment using ArgoCD
* Kubernetes-based scalable architecture
* Infrastructure provisioning using Terraform
* Automated deployments using ArgoCD Image Updater
* Integrated monitoring and observability

---

## ⚙️ CI/CD Pipeline

This project implements a CI/CD workflow to automate build and deployment:

* Source code pushed to GitHub
* CI pipeline builds Docker images
* Images pushed to container registry (ECR)
* Deployment triggered via GitOps using ArgoCD

---

## 📂 Project Structure

.
├── argocd/
├── terraform/
├── kubernetes-manifests/
├── helm-chart/
├── observability/
├── src/
├── docs/
└── README.md

---

## 🔁 Workflow

1. Developer pushes code to GitHub
2. CI pipeline builds and pushes Docker images
3. ArgoCD detects changes in Kubernetes manifests
4. Application is deployed automatically to AWS EKS
5. Monitoring tools track system health

---

## 📊 ArgoCD Deployment View

![image.png](docs/images/image%203.png)


---

## 👨‍💻 My Contributions

* Customized and structured the project for production-like deployment
* Integrated GitOps workflow using ArgoCD
* Configured Kubernetes manifests for microservices deployment
* Implemented CI/CD pipeline for automated build and deployment
* Organized repository for better readability and real-world usage

---
## 🎯 Problem Statement

Modern applications require scalable, reliable, and automated deployment systems. Managing microservices manually in production environments leads to challenges such as:

* Deployment inconsistencies across environments
* Lack of automation in CI/CD pipelines
* Difficulty in managing Kubernetes configurations
* Limited visibility and monitoring of applications

This project addresses these challenges by implementing a GitOps-driven DevOps workflow using Kubernetes (EKS), CI/CD pipelines, and ArgoCD for automated deployments.

---

## 💡 Solution Approach

To solve these challenges, this project implements:

* **GitOps Model** → Source of truth in Git, automated deployment via ArgoCD
* **CI/CD Pipeline** → Automated build, test, and deployment using Jenkins / GitHub Actions
* **Containerization** → Dockerized microservices for portability
* **Kubernetes (EKS)** → Scalable orchestration platform
* **Infrastructure as Code** → Terraform for automated provisioning
* **Observability** → Monitoring using Prometheus and Grafana

This ensures a fully automated, scalable, and production-ready deployment pipeline.

---

## 🌍 Real-World Use Case

This architecture is similar to how modern companies deploy applications in production environments, where:

* Developers push code changes to Git
* CI/CD pipelines automatically build and validate changes
* GitOps tools (ArgoCD) deploy updates to Kubernetes clusters
* Monitoring tools track system health and performance

This project simulates a real-world DevOps environment used in enterprise applications.


## 🧠 Key Learnings

* Hands-on experience with GitOps (ArgoCD)
* Built CI/CD pipelines for microservices
* Deployed applications on AWS EKS
* Worked with Terraform for infrastructure provisioning
* Implemented monitoring using Prometheus and Grafana

---

## 🚀 Future Improvements

* Implement service mesh (Istio)
* Add DevSecOps security scanning
* Multi-environment deployment (Dev / QA / Prod)
* Improve auto-scaling and resilience

---

## 👨‍💻 Author

**Srinivasulu**
DevOps Engineer | AWS | Kubernetes | Terraform | GitOps

---

## ⭐ Note

This project is built as part of hands-on DevOps practice to simulate real-world production environments and workflows.
