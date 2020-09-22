## What is Docker Image?

A Docker image is a read-only template that contains a set of instructions for creating a container that can run on the Docker platform. It provides a convenient way to package up applications and preconfigured server environments, which you can use for your own private use or share publicly with other Docker users.

A Docker image is a file, comprised of multiple layers, that is used to execute code in a Docker container. An image is essentially built from the instructions for a complete and executable version of an application, which relies on the host OS kernel.

## Structure of Docker File:

![Docker File Architecture](https://github.com/Ayushmanglani/Docker/blob/master/DockerImages/LayeredArchitecture.JPG)

## How Docker File Actually Looks?

![Docker File](https://github.com/Ayushmanglani/Docker/blob/master/DockerImages/dockerfile.JPG)

## Steps to create Docker Image:

 - <b>Step 1<u>: Create a directory and Enter in that Directory
    
    ```mkdir my-docker```
    
    ```cd my-docker```

 - <b>Step 2<u>: Create Docker file
 
    ```cat > Dockerfile ```     
 
 - <b>Step 3<u>: Create the Docker File: 
    This is a simple web application using Python Flask and MySQL database.
   - i.	Mention Operating System:
  
     ```FROM ubuntu ```
