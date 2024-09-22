# rancher-kubernetes

Rancher Kubernetes Engine (RKE) is a user-friendly, CNCF-certified Kubernetes setup that runs completely within Docker containers. Whether you’re on bare-metal or virtual servers, RKE makes installing and managing Kubernetes straightforward and automated. The best part? It’s flexible and works no matter what operating system or platform you’re using.

![image](https://github.com/user-attachments/assets/c30f6366-6655-4563-9a1b-16c48622caac)


## pre-req

rke and kubectl need for installation.

rke binary you can install (meanwhile 1.6.2 for this repo)

https://github.com/rancher/rke/releases/tag/v1.6.2

for kubectl you can follow documentation

https://kubernetes.io/docs/tasks/tools/#install-kubectl

your server need access via 22 port with private key

![image](https://github.com/user-attachments/assets/16eb7d5c-d031-4920-838a-c40d116810f3)


## configuration and install

rke use configuration yaml file you can find inside repo as configuration.yaml

then simple run below command.

```rke up --config ./rancher-cluster.yml```

## test

rancher put config file as kube_config_cluster.yml 

you can copy on .kube/config and 

```kubectl get nodes``` 
