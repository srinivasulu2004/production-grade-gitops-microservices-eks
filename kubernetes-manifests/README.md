
# 📦 Kubernetes Manifests

## 📌 Overview

This directory contains Kubernetes manifests for deploying the microservices-based application on a Kubernetes cluster (AWS EKS).

Each service is defined with its own Deployment and Service configuration to enable independent scaling, fault isolation, and seamless communication.

---

## 🧩 Microservices Included

The following services are deployed using these manifests:

* Frontend Service
* Product Catalog Service
* Cart Service
* Checkout Service
* Payment Service
* Currency Service
* Email Service
* Ad Service
* Load Generator (for testing traffic)

---

## ⚙️ Components

Each service typically includes:

* **Deployment** → Manages pod lifecycle and scaling
* **Service** → Exposes the application internally within the cluster

---

## 🚀 Deployment Steps

Apply all manifests using:

```bash
kubectl apply -f .
```

Verify deployment:

```bash
kubectl get pods
kubectl get svc
```

---

## 🔁 How it Works

* Each YAML file defines a microservice
* Kubernetes creates pods using container images
* Services enable communication between microservices
* Load is distributed across pods automatically

---

## 📊 Scaling

You can scale any service using:

```bash
kubectl scale deployment <service-name> --replicas=3
```

---

## 🧠 Key Concepts Demonstrated

* Kubernetes Deployments & Services
* Microservices architecture
* Pod scaling and load balancing
* Service discovery within cluster

---

## ⭐ Note

These manifests are integrated with GitOps (ArgoCD), where changes pushed to GitHub are automatically deployed to the Kubernetes cluster.
