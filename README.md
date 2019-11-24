# Docker

create a container and prints hash id of container
docker create hello-world

#watches the output of the conatiner and prints in console
docker start -a <hash-id>
prints the log which have emitted by container but does not resratr the container
docker logs <container-id> 

docker run <container> <command>
docker run busybox ls
docker run busybox echo hello

list all running container
docker ps

history of  all container which has been run 
docker ps --all

starting  a stopped container
runs the process which was provided during startup and can be changed
docker start -a <container-id> 


delete all stopped conatiner
docker system prune


running commands inside container
create a redis container
docker run redis

To run command inside container like redis cli

docker exec -it <container-id> <command>
docker exec -it <container-id> redis-cli

Tag an image 
docker build -t <docker-id>/name:<latest/name-version> <file-folder>