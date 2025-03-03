## 🚀 K8Demo App

### 📌 Overview

K8Demo is a simple application deployed on a lightweight K3s Kubernetes cluster. The CI/CD pipeline is managed using Jenkins, automating the build, test, and deployment process.

### 📌 Features

- ✅ Runs on K3s, a lightweight Kubernetes distribution
- ✅ CI/CD powered by Jenkins
- ✅ Automated deployment using Helm
- ✅ Ingress support for external access
- ✅ Dockerized application
  
---

### ⚙️ Tech Stack

- ✅ Kubernetes (K3s)
- ✅ Jenkins CI/CD
- ✅ Docker
- ✅ Nginx (Ingress)
- ✅ ArgoCD
  
---

### 🛠️ Setup Instructions

1️⃣ Prerequisites

Before you begin, ensure you have the following installed:

- K3s (Lightweight Kubernetes)
- Helm (Optional)
- Docker (For containerizing the app)
- Jenkins (For CI/CD automation)
- kubectl (Kubernetes CLI)
---

### 🚀 CI/CD Pipeline with Jenkins

The Jenkins pipeline (Jenkinsfile) is set up to:

- Pull the latest code from GitHub
- Build a Docker image and push to Docker Hub
- Deploy the app to K3s using Helm

Configure Jenkins Pipeline

1. Install required Jenkins plugins:
      - Pipeline
      - Kubernetes CLI
      - Docker Pipeline
2. Create a Jenkinsfile in the repo:
3. Add the pipeline in Jenkins → New Item → Pipeline
4. Configure GitHub Webhooks for automated triggers

---

### 🔍 Access the Application

Once deployed, check the service:
```
kubectl get svc k8demo
```

If using an Ingress, access it via the configured domain.
---

### 📜 License

This project is licensed under the MIT License.
📬 Contact

For issues or feature requests, open an issue or reach out to Sourish Bhattacharya.