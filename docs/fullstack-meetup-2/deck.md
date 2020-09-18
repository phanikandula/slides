### Docker for Full Stack Engineers

> Phani Kandula



### Introduction


About me


About you



## Agenda
- What is docker?
- What developer use cases does it support?
- Demo
- Troubleshooting tips



## Docker?

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



## Basic Idea

- Dockerfile             -- like a Hello.java file
- Docker Image           -- like a Hello.class file
- Docker Container       -- like an instance of Hello class
- Docker compose file    -- like constructor parameters for one Hello instance



## Demo time!

- docker run hello-world
- docker container run ubuntu cat /etc/hosts
- docker run -it ubuntu bash
- Develop on java code with IDE from inside docker
- Develop on maria DB with web frontend (adminer)



## Troubleshooting

Tip #1 - always do docker-compose config to verify file is correct


Tip #2 - always use docker-compose if you can and skip typing errors with long docker commands


Tip #3 - start containers in detached mode so that you are not tied to terminal


Tip #4 - Set up your application to redirect stdout and stderr to log files


Tip #5 - rebuild images if your code has changed otherwise you'll be surpised by seeing old functionality



## Resources

- https://training.play-with-docker.com/