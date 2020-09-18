### Kubernetes Introduction and Demo

> Phani Kandula



### Introduction


About me


About you



## Agenda
- Announcements
- Why Containers?
- Why Container Orchestration?
- Kubernetes: history, overview and architecture.
- Demo with minikube



## Announcements
- Please take survey: https://www.fullstacksoftwareengineer.com/survey
- Speak at this meetup: https://www.fullstacksoftwareengineer.com/speak 
- Silence phones etc.
- Active participation encouraged! Interrupt anytime..



## Why Containers?
Vendors:
- Docker
- rkt
- lxc
- Mesos


Docker containers wrap everything your application needs to run: 
 - code, 
 - runtime, 
 - system tools and
 - libraries.


## Docker vs Virtual Machine
- light weight vs heavy weight
- Metaphor: multiple shipping containers vs just one container on a ship


## Developer use cases


Onboard faster and stop wasting hours trying to set up development environments.


Spin up new instances and make copies of production code to run locally. Good for debugging.


Enable polyglot (full-stack) development and use any language, stack or tools without worry of application conflicts.


Eliminate environment inconsistencies and the "works on my machine" problem. 



## Why Container Orchestration?

- Define relationship between containers
- Where do containers come from
- How do we scale them
- How do they interact with the world



### Predecessor to Container Orchestration
- Homegrown scripts
- Manual configuration between containers



### Vendors
- Kubernetes
- Docker Swarm
- Mesos
- ECS, Azure, Digital Ocean



### Kubernetes - History
- Born from Google internal project (Borg)
- Abbreviated as k8 - Greek for 'helmsman' or 'pilot'
- Offered as open standard though Cloud Native Computing Foundation (CNCF)



### Kubernetes - Advantages
- Tested by Google for many years
- Very active community and governing organization (CNCF)
- Cloud agnostic



### Kubernetes - deployment options
- Evaluation/Training - minikube (local version of k8s)
- Development         - minikube with dev cluster on a cloud provider
- Deployment          - cloud provider or bare metal



### Concepts
- Deployments - akin to application
- Pods - instances of container in a deployment
- Services - end points exposed to outside world (ports)
- Nodes - machines that do the work of running containers



### Install (without virutualbox)
- Docker https://docs.docker.com/install/linux/docker-ce/ubuntu/
- Kubectl https://kubernetes.io/docs/tasks/tools/install-kubectl/
- Minikube https://kubernetes.io/docs/tasks/tools/install-minikube/



## Demo time!



## Manual process



### Run minikube
- sudo minikube start --vm-driver=none --apiserver-ips 127.0.0.1 --apiserver-name localhost
- sudo minikube status
- sudo minikube stop



### kubectl
- kubectl get pod
- kubectl run hello-minikube --image=k8s.gcr.io/echoserver:1.10 --port=8080
- kubectl expose deployment hello-minikube --type=NodePort
- curl $(minikube service hello-minikube --url)
- kubectl delete services hello-minikube
- kubectl delete deployment hello-minikube



## With deployment yaml file.
- kubectl apply -f deployment.yaml
- kubectl expose deployment tomcat-deployment --type=NodePort
- sudo minikube service tomcat-deployment --url
- kubectl delete services tomcat-deployment
- kubectl delete deployment tomcat-deployment



## With digital ocean.
- Create cluster on kubernetes Digital Ocean
- Download config file
- export KUBECONFIG=meetup-demo-config.yaml
- unset KUBECONFIG 



### Run tomcat and load balancer
- kubectl create -f deployment.yaml
- kubectl expose deployment tomcat-deployment --type=NodePort
- kubectl expose deployment tomcat-deployment --type=LoadBalancer --name=my-service
- kubectl get services my-service
- kubectl describe services
- kubectl delete services my-service
- kubectl delete services tomcat-deployment
- kubectl delete deployment tomcat-deployment
