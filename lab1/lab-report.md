University: ITMO University
Faculty: FICT
Course: Introduction to distributed technologies
Year: 2022/2023
Group: K4112c
Author: Chen guanyuan
Lab: Lab1
Date of create: 20.10.2022
Date of finished: 03.11.2022


Minikube start：
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab1/%E5%9B%BE%E7%89%871.png)

writing a manifest to deploy a HashiCorp Vault "pod"
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab1/%E5%9B%BE%E7%89%877.png)

Apply manifest.yaml, exposed port,and port-forward servifce:
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab1/%E5%9B%BE%E7%89%872.png)
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab1/%E5%9B%BE%E7%89%873.png)

Using command kubectl logs vault then find root token in logs:
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab1/%E5%9B%BE%E7%89%875.png)
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab1/%E5%9B%BE%E7%89%876.png)
We can access to the vault:
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab1/%E5%9B%BE%E7%89%874.png)


The scheme of organization of containers and services:
![Alt text](https://github.com/RIGHT-WOOD/2022_2023-introduction_to_distributed_technologies-k4113c-Guanyuan_Chen/blob/main/lab1/%E6%9C%AA%E5%91%BD%E5%90%8D%E7%BB%98%E5%9B%BE.drawio)
