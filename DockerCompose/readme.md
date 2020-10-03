## Docker Compose

- Compose is a tool for defining and running multi-container Docker applications.
- Docker Compose is used to run multiple containers as a single service. 
- With Compose, you use a YAML file to configure your application’s services. Then, with a single command, you create and start all the services from your configuration.
- For Example, You Want to Run MongoDB Server and Flask server with connection between them, for this you could create one file (docker compose) which would start both the containers as a service without the need to start each one separately.






To Use a Docker Compose three-step process:

 1. Define your app’s environment with a Dockerfile so it can be reproduced anywhere.

 2. Define the services that make up your app in docker-compose.yml so they can be run together in an isolated environment.

 3. Run docker-compose up and Compose starts and runs your entire app
