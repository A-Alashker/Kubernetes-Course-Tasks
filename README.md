# Kubernetes-Course-Tasks

## 1. Create the cluster

```minikube start --driver=docker --cpus=2 --memory=4000 --nodes=3 --cni=calico```  
``` kubectl get nodes```            

## 2. Create namespace
<img width="1358" height="59" alt="image" src="https://github.com/user-attachments/assets/ce9042c2-2854-4873-ba6d-23cb64d4ff12" />

## 3. Write the Deployment yaml file

<img width="1360" height="653" alt="image" src="https://github.com/user-attachments/assets/d3c45fcd-9454-4227-bd3e-9dd5a64f03a3" />

## 4. Deploy and check

<img width="1360" height="368" alt="image" src="https://github.com/user-attachments/assets/f80dbe82-14d3-432c-8682-c8a9639f84d7" />


<img width="1082" height="340" alt="image" src="https://github.com/user-attachments/assets/fe9f5832-949f-46eb-aa6a-99ebdc308daf" />


<img width="1358" height="694" alt="image" src="https://github.com/user-attachments/assets/9e9e73db-6f9e-4e79-ac94-fe4edcde222d" />

### after 10 seconds

<img width="1358" height="694" alt="image" src="https://github.com/user-attachments/assets/3764d2ce-1e35-491c-abe4-48a0c6fc4ec3" />

## 5. Make the init container fail

<img width="1358" height="221" alt="image" src="https://github.com/user-attachments/assets/8bb03e8e-3620-41d8-881a-6aeeb2bc92a4" />

<img width="1358" height="578" alt="image" src="https://github.com/user-attachments/assets/ca58fb47-62b6-43da-b01a-4d363371c88e" />

<img width="1358" height="578" alt="image" src="https://github.com/user-attachments/assets/443808b3-6e94-4c45-b36a-12750ffcd160" />

<img width="1358" height="589" alt="image" src="https://github.com/user-attachments/assets/04c165ec-d2e3-43cb-adaa-db44081de5b4" />

<img width="1358" height="603" alt="image" src="https://github.com/user-attachments/assets/a2d6fd20-e24d-4089-b02e-a2285ad43ab0" />


### Q1: Which status does the new Pod show?

#### Init:Error and then Init:CrashLoopBackOff

### Q2: Do nginx and time-updater start?

#### No they don't 

### Q3: Is the page still reachable, and why?

#### No, because nginx container is not initiated (Init:Error)

## 6. Fix it

<img width="1355" height="546" alt="image" src="https://github.com/user-attachments/assets/d42537a4-1552-4917-b74a-c23192690a71" />

