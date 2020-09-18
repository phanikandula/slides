## JamStack Austin Meetup #4

Using Docker to create, build and host your JAMStack sites

> Phani Kandula



### Introduction


About me


About you



## Agenda
- Recap JAMStack!
- What is docker?
- What developer use cases does it support?
- Demo



## Recap!


JAMstack: noun \’jam-stak’\ 
- Modern web development architecture based on client-side JavaScript, reusable APIs, and prebuilt Markup.


Javascript
- Client side 
- Any framework or library or vanilla JS
- Handles request and processing dynamic data


API
- Abstracts server side processes and/or database access.
- Accessed with JS over HTTP
- Your custom API or 3rd party API or both.


Markup
- Prebuilt at deploy time



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
- write hugo blog posts inside docker
- serve staging version of blog posts with docker
- host live static site with docker
