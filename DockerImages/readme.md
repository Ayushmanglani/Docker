## What is Docker Image?

A Docker image is a read-only template that contains a set of instructions for creating a container that can run on the Docker platform. It provides a convenient way to package up applications and preconfigured server environments, which you can use for your own private use or share publicly with other Docker users.

A Docker image is a file, comprised of multiple layers, that is used to execute code in a Docker container. An image is essentially built from the instructions for a complete and executable version of an application, which relies on the host OS kernel.

## Structure of Docker File:

![Docker File Architecture](https://github.com/Ayushmanglani/Docker/blob/master/DockerImages/LayeredArchitecture.JPG)

## How Docker File Actually Looks?

![Docker File](https://github.com/Ayushmanglani/Docker/blob/master/DockerImages/dockerfile.JPG)

## Steps to create Docker Image:

 - <b>Step 1</b>: Create a directory and Enter in that Directory
    
    ```
    mkdir my-simple-docker
    ```
    
    ```
    cd my-docker
    ```

 - <b>Step 2</b>: Create Docker file:  This is a simple web application using Python Flask and MySQL database.
 
    ```
    cat > Dockerfile 
    ```     
 
 - <b>Step 3</b>: Update the created Docker File:     
   
    ```
    vi Dockerfile 
    ``` 
    
    Press 'i' (for cahnging mode to insert) and write the Docker File in Following way:
    
 
   - A.	Mention Operating System:
  
     ```FROM ubuntu ```

   - B.	Install all required dependencies
   
     ```
     RUN apt-get update
     
     RUN apt-get install –y python python-pip
     ```
   - C.	Install and Configure Web Server
     
     ```
     RUN pip install flask
     RUN pip install flask-mysql
     ```
     
   - D.	Create/Copy the Source/Application code into <b>/opt/app.py</b>
   
     ```
     COPY app.py /opt/app.py
     ```

   - E. Give Entry point
     ```
     ENTRYPOINT FLASK_APP-/opt/aap.py flask run –host-0.0.0.0
     ```
   - F. To save File and exit vim use, 'Esc', then type ```:wq``` and hit 'Enter'
   
   
 - <b>Step 4</b>: Create Application Code
 
   - A. Create app.py
     ```
     cat app.py 
     ```
    
   - B. Write Code   
     ```
     import os
     from flask import Flask
     app = Flask(__name__)

     @app.route("/")
     def main():
         return "Welcome!"

     @app.route('/how are you')
     def hello():
         return 'I am good, how about you?'

     if __name__ == "__main__":
         app.run(host="0.0.0.0", port=8080)     
     ```
     
 - <b>Step 5</b>:	Build the Image with tagging a name to it
 
     ```
     docker build . –t my-simple-docker
     ```
     
- <b>Step 6</b>:	Check whether the images is created

     ```
     docker images
     ```

- <b>Step 7</b>: Run the Docker image

     ```
     docker run –t my-simple-docker
     ```

- <b>Step 8</b>: If you want to push Image to Docker Hub:

   - A.	Tag image to your account  
     ```
     docker build . –t ayush/my-simple-docker 
     ```
     
   - B.	Login to your account   
     ```
     docker login
     ```
     
   - C.	Run push Comand
     ``` 
     docker push
     ```
     
- <b>Step 9</b>:	It's Done, Check the image in your dashboard on Dockerhub

   



