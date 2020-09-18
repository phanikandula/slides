### Kubernetes Part 5
All about networking!

> Phani Kandula



### Introduction


About me


About you



## Agenda
- Announcements
- Why not use just IP and ports
- Services - Cluster IP, NodePort and Loadbalancer
- Ingress and IngressController



## Announcements
- Please take survey: https://www.fullstacksoftwareengineer.com/survey
- Speak at this meetup: https://www.fullstacksoftwareengineer.com/speak 
- Silence phones etc.
- Active participation encouraged! Interrupt anytime..



## Usecases


External clients connect to internal pods


Internal clients connect to internal pods


Internal clients connect to external services


External clients connect to external services



## Why not use just IP and ports?


Pods are ephemeral


Pods can be scaled


Cannot know IP upfront


We can't reconfigure our clients everytime IP and port changes



## What are Services?

A resource that can guarantee constant IP and port

Allow pods to be found using service name:
- Using environment vars
- Using DNS



## Demos
- Show Pods IP changes when recreated
- Create services and access using env vars, DNS and IP
