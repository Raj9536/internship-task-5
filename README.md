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

minikube start

 **2. Created deployment.yaml for Nginx App**

kubectl apply -f deployment.yaml

**3. Created and Applied service.yaml to Expose the App**

kubectl apply -f service.yaml


**✅ 4. Verified Pods and Services**


kubectl get pods
kubectl get services

**✅ 5. Accessed the Application in Browser**

bash
Copy
Edit
minikube service myapp-service

**✅ 6. Scaled the Deployment**


kubectl scale deployment myapp-deployment --replicas=4
kubectl get pods

**✅ 7. Described Resources**


kubectl describe deployment myapp-deployment
kubectl describe service myapp-service
kubectl describe pod <pod-name>\


**Screenshots**

1. Starting Minikube
![minkube start](https://github.com/user-attachments/assets/9e70b10e-45a4-4b04-8af7-fd662f4e7d1a)

2. Seeing the running Pods
![get pods](https://github.com/user-attachments/assets/5e10d0a0-93b4-42ca-8fd5-366e646da976)

3. Seeing the running Services
![get services](https://github.com/user-attachments/assets/fcb9629b-5743-46b8-8c2d-f352029bc548)

4. Accesing the uploaded my-app on the browser
![accessing my services](https://github.com/user-attachments/assets/835aa3d4-a399-4cc4-8296-e2ff01083149)

5. Scaling up the Pods 
![scale up pods](https://github.com/user-attachments/assets/2f4e740c-8831-4a5b-bdd4-99c6db688416)

6. Using the describe command to get the more details about the pod, services, deployment
![pod describe](https://github.com/user-attachments/assets/484abdbd-2ba8-439c-8d59-19dfa268976d)

7. Finally deleting the deployment, services and stopping the minikube
![stop minikube](https://github.com/user-attachments/assets/e0deec5e-bbef-4a9a-a5cb-36efb1229f79)


**📘 Key Learnings**
Kubernetes deployment and service basics

Managing clusters with Minikube

Scaling and describing Kubernetes resources

Practical understanding of how Pods, Deployments, and Services work

**📂 Folder Structure**

![image](https://github.com/user-attachments/assets/c6d1c11b-7ad1-4103-bdf2-cd5dbf51280f)


**✅ Outcome**
Successfully deployed a containerized Nginx app on a local Kubernetes cluster using Minikube, and learned the workflow of deployments, services, scaling, and debugging using kubectl.
