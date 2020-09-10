Docker Commands:
•	docker run nginx – Runs a docker image, if docker image not present onhost, it pull the image from dockerhub, this happens only first time
•	docker ps – list dockers, with their details(name, status, id)
•	docker ps –a -> All running commands
•	docker stop -> stop running docke4r by providing it’s id or name
•	docker rm silly_sammet -> remove docker image
•	docker images -> dockers images available and their size
•	docker rmi nginx -> remove a docker from host
•	docker pullnginx – pull image to host, but doesn’t run it
•	docker exec distracted_mcclintock(docker id / docker_name) cat /etc/host -> execute a command on docker container
