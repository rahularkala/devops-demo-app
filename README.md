# 🚀 End-to-End CI/CD DevOps Pipeline Project

## 📌 Overview

This project demonstrates a complete DevOps pipeline integrating CI/CD, code quality, security scanning, containerization, and Kubernetes deployment using Helm.

---

## 🛠️ Tech Stack

* GitHub (Version Control)
* Jenkins (CI/CD Pipeline)
* SonarQube (Code Quality Analysis)
* Docker (Containerization)
* Trivy (Security Scanning)
* Kubernetes (Minikube) (Container Orchestration)
* Helm (Deployment Management)

---

## 🔄 Pipeline Flow

1. Developer pushes code to GitHub
2. Jenkins pipeline triggers automatically
3. Dependencies are installed
4. SonarQube performs code quality checks
5. Docker image is built
6. Trivy scans image for vulnerabilities
7. Application is deployed to Kubernetes using Helm

---

## 🐳 Docker

Build image:

```
docker build -t devops-demo .
```

Run container:

```
docker run -p 3000:3000 devops-demo
```

---

## ☸️ Kubernetes Deployment

```
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

---

## 📦 Helm Deployment

```
helm install my-app devops-chart
```

---

## 🔐 Security Scan

```
trivy image devops-demo
```

---

## 📊 SonarQube

* Detects bugs and code smells
* Improves maintainability and reliability

---

## 🧠 Key Learnings

* CI/CD pipeline automation
* Docker and container lifecycle
* Kubernetes deployment and debugging
* Helm chart creation and management
* Security scanning and vulnerability handling
* Real-world DevOps troubleshooting

---

## 🎯 Outcome

Successfully built a production-like CI/CD pipeline with automated build, test, scan, and deployment processes.

---

## 📌 Author

Rahul Arkala
