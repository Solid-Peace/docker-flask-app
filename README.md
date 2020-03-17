# Docker-Flask-App

A simple docker container project based on [this tutorial](https://github.com/docker/labs/blob/master/beginner/chapters/webapps.md)

See Dockerfile to have an overview of contructing of a docker image

## Commands lines

**Build Image**
`docker build -t <user-name>/docker-flask-app .`

**List Images**
`docker images`

**Run container from image**
`docker run -p 8888:5000 --name test <user-name>/docker-flask-app`

**Save image**
`docker save <user-name>/docker-flask-app > docker-flask-app-image.tar`

**Load image**
`docker load < docker-flask-app-image.tar`

**Docker containers is runing**
`docker ps`


**Stop container with name or id**
```
docker stop test
docker rm test

or

docker rm -f test
```