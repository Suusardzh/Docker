# Docker
Docker basics

## Docker Commands

Remove all containers
```
docker rm $(docker ps -aq)
```
​
Remove all images
```
docker rmi $(docker images -aq)
```

Stop all running containers
```
docker stop $(docker ps -aq)
```
### List all images
```
docker images
```
### Run container with centos latest image
```
docker run centos
```
### Pull ubuntu 18.04d image 
```
docker pull ubuntu:18.04d
```
### List running containers
```
docker ps
```
### List all containers
```
docker ps -a
```
### Run container with nginx image in the background
```
docker run -d nginx
```
### Create whale
```
docker run docker/whalesay cowsay boo  
```
### Remove ubuntu image
```
docker rmi ubuntu 
```
### Execute to ansible_master container
```
docker exec -it ansible_master bash
```
## Resources

[Link to Katacoda](https://katacoda.com/courses/docker/deploying-first-container)

[Link to Docker Commit](https://docs.docker.com/engine/reference/commandline/commit/)