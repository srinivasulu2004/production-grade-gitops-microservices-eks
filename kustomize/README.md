# ⚙️ Kustomize Configuration

## 📌 Overview

This directory contains Kustomize configurations used to manage and customize Kubernetes manifests for deploying the microservices application.

Kustomize helps in modifying Kubernetes resources without duplicating YAML files, enabling environment-specific configurations and reusable components.

---

## 🧩 What is Kustomize?

Kustomize is a Kubernetes configuration management tool that allows customization of manifests using overlays and components.

It is built into `kubectl` and can be used with:

```bash
kubectl apply -k .
```

---

## 📂 Structure

* `kustomization.yaml` → Main configuration file
* `base/` → Base Kubernetes manifests
* `components/` → Optional reusable configurations

---

## 🚀 Usage

### Preview manifests

```bash
kubectl kustomize .
```

### Apply configuration

```bash
kubectl apply -k .
```

---

## 🔁 How it Works

* Base manifests define core services
* Kustomize overlays modify configurations
* Changes are applied dynamically without editing original YAML files
* Integrated with GitOps (ArgoCD) for automated deployment

---

## 🧠 Key Concepts

* Base and overlays
* Reusable components
* Environment-specific configurations
* GitOps-friendly deployment

---

## ⭐ Note

This setup is integrated with ArgoCD, where updates to the repository automatically trigger deployments to the Kubernetes cluster.
