### Kubernetes from the ground up: Part 1

> Phani Kandula



### Introduction


About me


About you



## Agenda
- Announcements
- Why Kubernetes?
- Docker from zero



## Announcements
- Please take survey: https://www.fullstacksoftwareengineer.com/survey
- Speak at this meetup: https://www.fullstacksoftwareengineer.com/speak 
- Silence phones etc.
- Active participation encouraged! Interrupt anytime..



## Why Kubernetes?
Kubernetes provides four important values:
- Velocity
- Scaling
- Abstraction of infrastructure
- Efficiency


## Velocity
Number of things you can ship while maintaining a highly available service.

- Immutability
- Declarative config
- Self healing system


## Scaling
- Decouple containers from machines (nodes)
- Make micro-services easy
- Load balancing


## Abstraction of infrastructure
- Multi-cloud
- Hybrid cloud
- Full control of services


## Efficiency
- Multiple containers on one machine
- Less time to deploy or update
- Quickly create dev and test clusters
- Continuous integration



## Docker allows to package:
- OS (alpine) with packages (ssl)
- Programming language runtime (python 3.6.8)
- Packages the application needs (python requests, flask)
- Tools needed to run the program (uwsgi)



## Demos
- Serve html
- Serve dummy json api
- Monitor docker
- Develop webapp without installing dependencies