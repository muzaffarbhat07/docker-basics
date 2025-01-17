## Basics of Docker

### Why Containerisation?
1. Everyone has different Operating systems
2. Steps to run a project can vary based on OS
3. Extremely harder to keep track of dependencies as project grows
4. What if there was a way to describe your projects configuration in a single file?
5. What if that could be run in an isolated environment
6. Makes Local setup of projects a breeze
7. Makes installing auxiliary services easy

##### MEME:
- IT WORKS ON MY MACHINE 
- THEN WE'LL SHIP YOUR MACHINE
- ANS THAT IS HOW DOCKER WAS BORN

### What is Containerisation?

Containerization involves building self-sufficient software packages that perform consistently, regardless of the machines they run on.

It's basically taking the snapshot of a machine, the filesystem and letting you use and deploy it as a construct


### History of Docker
1. Introduced in 2014
2. Caught on fire 2015 onwards
3. Most open source projects have docker
4. Makes your life easy when you're setting locally
5. Makes it easier to deploy containers
6. Allows for container orchestration which makes deployment a breeze


### Installing Docker:
  https://docs.docker.com/engine/install/


### Inside Docker

##### Docker has 3 parts:
1. CLI
2. Engine: Docker daemon - main part -> lets create images etc
3. Registry (maily, docker hub): deploy images to docker hub, then pull from other places to run


### Images vs Containers

A Docker "image" behaves like a template from which consistent containers can be created. If
Docker was a traditional virtual machine, the image could be likened to the ISO used to install your
VM. This isn't a robust comparison, as Docker differs from VMs in terms of both concept and
implementation, but it's a useful starting point nonetheless.

Images define the initial filesystem state of new containers. They bundle your application's source
code and its dependencies into a self-contained package that's ready to use with a container
runtime. Within the image, filesystem content is represented as multiple independent layers.

In short, Image is a snapshot and image in execution is a container. We can create multiple containers from a single image.
