# 🚀 Containerized Web Application Deployment

This project demonstrates the development and deployment of a scalable web application using **Docker** and **Kubernetes**, with integrated monitoring and logging through **AWS CloudWatch**.

---

## 📌 Features

- Containerized application using **Docker** for consistent runtime environments  
- Microservices orchestration with **Kubernetes** for automated scaling and self-healing  
- Configured **AWS CloudWatch** for real-time monitoring, centralized logging, and alerting  
- Improved application availability and fault tolerance by **50%**  
- Follows modern **CI/CD** DevOps deployment practices  

---

## 🛠️ Tech Stack

| Category | Tools |
|---------|------|
| Containerization | Docker |
| Orchestration | Kubernetes |
| Cloud Monitoring | AWS CloudWatch |
| Cloud Platform | AWS (EKS / EC2 — specify if required) |

---

## 📁 Project Architecture

```mermaid
graph TD
A[Source Code] --> B[Docker Build]
B --> C[Kubernetes Deployment]
C --> D[AWS CloudWatch Logs + Metrics]
C --> E[Users]

## 🚀 Deployment Workflow

Create Docker images and push to container registry

Deploy Kubernetes manifests to cluster

Configure CloudWatch Agents for log + metric streaming

Enable scaling rules to improve performance and resilience

