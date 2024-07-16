# docker 
 In this we will learn about docker and containerization 

 
What is a container ?

A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. 
A container is a bundle of Application, Application libraries required to run your application and the minimum system dependencies.

Why are containers light weight ?
Containers are lightweight because they use a technology called containerization, which allows them to share the host operating system's kernel and libraries, while still providing isolation for the application and its dependencies.

What is Docker ?

Docker is a containerization platform that provides easy way to containerize your applications, which means, using Docker you can build container images, run the images to create containers and also push these containers to container regestries such as DockerHub

what is Docker container ?

A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

Docker LifeCycle

There are three important things,

docker build -> builds docker images from Dockerfile
docker run -> runs container from docker images
docker push -> push the container image to public/private regestries to share the docker images.

Dockerfile ?

Dockerfile is a file where you provide the steps to build your Docker Image.

Images 

An image is a read-only template with instructions for creating a Docker container





 
