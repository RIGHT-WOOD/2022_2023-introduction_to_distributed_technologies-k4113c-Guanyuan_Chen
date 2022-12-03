University: ITMO University

Faculty: FICT

Course: Introduction to distributed technologies

Year: 2022/2023

Group: K4112c

Author: Chen guanyuan

Lab: Lab2

Date of create: 20.10.2022

Date of finished: 03.11.2022

Minikube start：
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab2/2.png)

Creating a deployment manifest:
https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab2/weblab.yaml

Apply deployment:
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab2/2.png)

View pod status:
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab2/3.png)

Creating a service manifest:
https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab2/weblabsev.yaml

Creating a service through which we will have access to these "pods":
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab2/4.png)

minikube kubectl -- expose deployment/webserver --type=NodePort --port=3000
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab2/4.5.png)
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab2/6.png)

Now, we can access to website via link http://localhost:3000:
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab2/7.png)
