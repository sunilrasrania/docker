# Docker 
 In this we will learn about docker and containerization 

 
**What is a container ?**

A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. 
A container is a bundle of Application, Application libraries required to run your application and the minimum system dependencies.

**Why are containers light weight ?**

Containers are lightweight because they use a technology called containerization, which allows them to share the host operating system's kernel and libraries, while still providing isolation for the application and its dependencies.

**What is Docker ?**

Docker is a containerization platform that provides easy way to containerize your applications, which means, using Docker you can build container images, run the images to create containers and also push these containers to container regestries such as DockerHub

**DOCKER CONTAINER**

A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

**Docker LifeCycle**

There are three important things,

docker build -> builds docker images from Dockerfile
docker run -> runs container from docker images
docker push -> push the container image to public/private regestries to share the docker images.

**Dockerfile ?**

Dockerfile is a file where you provide the steps to build your Docker Image.

**Images**

An image is a read-only template with instructions for creating a Docker container

## INSTALL DOCKER

A very detailed instructions to install Docker are provide in the below link

https://docs.docker.com/get-docker/ 

For Demo,
You can create an Ubuntu EC2 Instance on AWS and run the below commands to install docker.

`sudo apt update`

`sudo apt install docker.io -y`

A easy way to verify your Docker installation is by running the below command

`docker run hello-world`

If the output says:

`docker: Got permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Post "http://%2Fvar%2Frun%2Fdocker.sock/v1.24/containers/create": dial unix /var/run/docker.sock: connect: permission denied.
See 'docker run --help'.`

This can mean two things,

Docker deamon is not running.
Your user does not have access to run docker commands.

Start Docker daemon

`sudo systemctl status docker`

`sudo systemctl start docker`

Grant Access to your user to run docker commands

`sudo usermod -aG docker ubuntu`

In the above command ubuntu is the name of the user, you can change the username appropriately.

**Docker is Installed, up and running 🥳🥳**

docker run hello-world

**output**

>....
>....

Hello from Docker!
This message shows that your installation appears to be working correctly.
>...
>...

**Build your first Docker Image**

### Commands

`docker build -t (name) image:latest.`

**Verify Docker Image is created**

`docker images`

**Run your First Docker Container**

`docker run -it (image name)`

**Push the Image to DockerHub and share it with the world**

`docker push (image-name)`

**this is all about docker**

#### DRAWBACK OF DOCKER 

1. DOCKER DEAMONS ITSELF RUNS WITH A ROOT USER

2. IT IS A SINGLE PROCESS OR MONILOTHIC PROCESS


