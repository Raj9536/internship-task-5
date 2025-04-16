# 🚀 Task 5 - Kubernetes Cluster with Minikube

## 📌 Objective
Deploy and manage applications in a Kubernetes cluster using Minikube, kubectl, and Docker.

---

## 🛠 Tools Used
- Minikube
- kubectl
- Docker
- Windows PowerShell

---

## 🧩 Task Steps

### ✅ 1. Installed Minikube & Started the Cluster
```bash
minikube start

 **2. Created deployment.yaml for Nginx App**

kubectl apply -f deployment.yaml

**3. Created and Applied service.yaml to Expose the App**
kubectl apply -f service.yaml

✅ 4. Verified Pods and Services
bash
Copy
Edit
kubectl get pods
kubectl get services
✅ 5. Accessed the Application in Browser
bash
Copy
Edit
minikube service myapp-service
✅ 6. Scaled the Deployment
bash
Copy
Edit
kubectl scale deployment myapp-deployment --replicas=4
kubectl get pods
✅ 7. Described Resources
bash
Copy
Edit
kubectl describe deployment myapp-deployment
kubectl describe service myapp-service
kubectl describe pod <pod-name>
📸 Screenshots
![minkube start](https://github.com/user-attachments/assets/4de44197-fc40-43fa-a8d1-71a7f3310689)


![get pods](https://github.com/user-attachments/assets/f5f72761-0f89-4767-9615-1f4bc9573956)


![get services](https://github.com/user-attachments/assets/bfaad686-0bca-4264-b695-b5f0db7d39b0)


![accessing my services](https://github.com/user-attachments/assets/930e3366-5734-4b42-aeae-79a1e20001de)


![scale up pods](https://github.com/user-attachments/assets/74619bfe-ce87-4806-bb6f-45bbb0a50645)


![pod describe](https://github.com/user-attachments/assets/b283e460-ddfa-45c2-8978-f9552dd75ddb)


![stop minikube](https://github.com/user-attachments/assets/2c9f1674-6741-4e37-a648-145acd9fc5ac)

📘 Key Learnings
Kubernetes deployment and service basics

Managing clusters with Minikube

Scaling and describing Kubernetes resources

Practical understanding of how Pods, Deployments, and Services work

📂 Folder Structure
pgsql
Copy
Edit
.
├── deployment.yaml
├── service.yaml
├── screenshots/
│   ├── minikube-start.png
│   ├── get-pods.png
│   ├── get-services.png
│   └── nginx-browser.png
└── README.md
✅ Outcome
Successfully deployed a containerized Nginx app on a local Kubernetes cluster using Minikube, and learned the workflow of deployments, services, scaling, and debugging using kubectl.
