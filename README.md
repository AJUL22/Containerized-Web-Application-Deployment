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






## Contributing
Guidelines for collaborators.

## License
Project license details.




# Build & push
docker build -t myapp:version .
docker push repo/myapp:version

# Create EKS cluster
eksctl create cluster --name myapp-cluster --region eu-central-1 --nodes 3

# Deploy to k8s
kubectl apply -f deployment.yaml
kubectl get pods,svc

# Autoscale
kubectl autoscale deployment myapp-deploy --cpu-percent=60 --min=2 --max=10

# Install logging
helm repo add aws-for-fluent-bit https://aws.github.io/eks-charts
helm repo update
helm install fluent-bit aws-for-fluent-bit/aws-for-fluent-bit --set clusterName=myapp-cluster

# Check logs (CloudWatch) via AWS console

