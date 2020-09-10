# Docker Commands:

| Command | Description | Example | 
| --- | --- | --- |
|	docker attach	|	Attach local standard input, output, and error streams to a running container	| docker attach topdemo |
|	docker build	|	Build an image from a Dockerfile	| docker build http://server/context.tar.gz |
|	docker builder	|	Manage builds	| docker builder build |
|	docker checkpoint	|	Manage checkpoints	| docker checkpoint create |
|	docker commit	|	Create a new image from a container’s changes	| docker commit containerid | 
|	docker config	|	Manage Docker configs	| docker config create |
|	docker container	|	Manage containers	|	docker container attach	|
|	docker context	|	Manage contexts	|	docker context create	|
|	docker cp	|	Copy files/folders between a container and the local filesystem	|	docker cp [OPTIONS] CONTAINER:SRC_PATH DEST_PATH	|
|	docker create	|	Create a new container	|	docker create [OPTIONS] IMAGE [COMMAND] [ARG...]	|
|	docker diff	|	Inspect changes to files or directories on a container’s filesystem	|	docker diff CONTAINER	|
|	docker events	|	Get real time events from the server	|	docker events [OPTIONS]	|
|	docker exec	|	Run a command in a running container	|	docker exec [OPTIONS] CONTAINER COMMAND	|
|	docker export	|	Export a container’s filesystem as a tar archive	|	docker export [OPTIONS] CONTAINER	|
|	docker history	|	Show the history of an image	|	docker history [OPTIONS] IMAGE	|
|	docker image	|	Manage images	|	docker image COMMAND	|
|	docker images	|	List images	|	docker images [OPTIONS]	|
|	docker import	|	Import the contents from a tarball to create a filesystem image	|	docker import http://example.com/exampleimage.tgz	|
|	docker info	|	Display system-wide information	|	docker info [OPTIONS]	|
|	docker inspect	|	Return low-level information on Docker objects	|	docker inspect [OPTIONS] NAME	|
|	docker kill	|	Kill one or more running containers	|	docker kill [OPTIONS] CONTAINER	|
|	docker load	|	Load an image from a tar archive or STDIN	|	docker load [OPTIONS]	|
|	docker login	|	Log in to a Docker registry	|	docker login [OPTIONS] [SERVER]	|
|	docker logout	|	Log out from a Docker registry	|	docker logout [SERVER]	|
|	docker logs	|	Fetch the logs of a container	|	docker logs [OPTIONS] CONTAINER	|
|	docker manifest	|	Manage Docker image manifests and manifest lists	|	docker manifest COMMAND 	|
|	docker network	|	Manage networks	|	docker network COMMAND	|
|	docker node	|	Manage Swarm nodes	|	docker node COMMAND	|
|	docker pause	|	Pause all processes within one or more containers	|	docker pause CONTAINER	|
|	docker plugin	|	Manage plugins	|	docker plugin COMMAND	|
|	docker port	|	List port mappings or a specific mapping for the container	|	docker port CONTAINER	|
|	docker ps	|	List containers	|	docker ps	|
|	docker pull	|	Pull an image or a repository from a registry	|	docker pull [OPTIONS] NAME	|
|	docker push	|	Push an image or a repository to a registry	|	docker push [OPTIONS] NAME	|
|	docker rename	|	Rename a container	|	docker rename CONTAINER NEW_NAME	|
|	docker restart	|	Restart one or more containers	|	docker restart [OPTIONS] CONTAINER	|
|	docker rm	|	Remove one or more containers	|	docker rm [OPTIONS] CONTAINER	|
|	docker rmi	|	Remove one or more images	|	docker rmi [OPTIONS] IMAGE	|
|	docker run	|	Run a command in a new container	|	docker run [OPTIONS] IMAGE	|
|	docker save	|	Save one or more images to a tar archive (streamed to STDOUT by default)	|	docker save [OPTIONS] IMAGE	|
|	docker search	|	Search the Docker Hub for images	|	docker search [OPTIONS] TERM	|
|	docker secret	|	Manage Docker secrets	|	docker secret COMMAND	|
|	docker service	|	Manage services	|	docker service COMMAND	|
|	docker stack	|	Manage Docker stacks	|	docker stack [OPTIONS] COMMAND	|
|	docker start	|	Start one or more stopped containers	|	docker start [OPTIONS] CONTAINER 	|
|	docker stats	|	Display a live stream of container(s) resource usage statistics	|	docker stats [OPTIONS] [CONTAINER...]	|
|	docker stop	|	Stop one or more running containers	|	docker stop [OPTIONS] CONTAINER	|
|	docker swarm	|	Manage Swarm	|	docker swarm COMMAND	|
|	docker system	|	Manage Docker	|	docker system COMMAND	|
|	docker tag	|	Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE	|	docker tag SOURCE_IMAGE[:TAG] TARGET_IMAGE[:TAG]	|
|	docker top	|	Display the running processes of a container	|	docker top CONTAINER	|
|	docker trust	|	Manage trust on Docker images	|	docker trust COMMAND	|
|	docker unpause	|	Unpause all processes within one or more containers	|	docker unpause CONTAINER	|
|	docker update	|	Update configuration of one or more containers	|	docker update [OPTIONS] CONTAINER	|
|	docker version	|	Show the Docker version information	|	docker version [OPTIONS]	|
|	docker volume	|	Manage volumes	|	docker volume create [OPTIONS] [VOLUME]	|
|	docker wait	|	Block until one or more containers stop, then print their exit codes	|	docker wait CONTAINER	|
