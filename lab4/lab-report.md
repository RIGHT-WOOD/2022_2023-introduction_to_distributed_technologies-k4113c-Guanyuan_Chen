University: ITMO University

Faculty: FICT

Course: Introduction to distributed technologies

Year: 2022/2023

Group: K4112c

Author: Chen guanyuan

Lab: Lab4

Date of create: 20.10.2022

Date of finished: 30.11.2022

Creating a minikube cluster with 2 nodes and install the CNI=calico plugin
minikube start --network-plugin=cni --cni=calico --nodes 2 --kubernetes-version=v1.24.0 and Minikube node add
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab4/1.png)

Get the list of created nodes:
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab4/2.png)
Set labels for nodes:
kubectl label nodes minikube zone=west
kubectl label nodes minikube-m02 zone=you
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab4/3.png)

Create ippool with 2 labels in step 4: kubectl apply -f ip.yaml Create deployment with 2 replicaset and env: kubectl apply -f lab-ip.yaml Ceate service for deployment: kubectl apply -f weblabsev.yaml
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab4/4.png)
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab4/5.png)

Result
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab4/6.png)


The scheme of organization of containers and services:
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab4/lab4.png)
