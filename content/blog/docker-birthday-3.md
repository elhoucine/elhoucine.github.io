+++

date = "2016-03-23T20:46:03Z"

draft = false

title = "docker birthday 3"

+++


Hello It's Docker's year 3 :D, celebrations everywhere.

We @ Casablanca, had a Docker session by @SamuelTerburg.

Special thanks to him, and to the guys behind the event.
<!-- Docker project & Docker Inc(Business -->
<!-- dockerCon16 -->

# Quick notes.

## Docker Component:

* Docker Image should contains all dependencies.
* Docker container => secure, (Bundle the Docker image)
* Docker Engine run the Docker container.

## Docker services:

* Docker Swarm: Orchestrator to manage Docker container in a cluster.

## Docker power:
* Isolation.
* Dependencies.
* Security
* Speed.
* Portability.
* Performance.

<!-- Docker data center VS Docker Cloud. -->

<!-- Docker alpine : Base docker image with basic system requirement. (5mb) -->

### Docker commands:

`docker images`

`docker ps`

`docker run image_name`

`docker run alpine sh`

`docker run -d alpine sh  #run the container as a daemon`

`docker ps -a  #List docker images`

`docker log sharp_banach`

`docker stop image_name`

`docker run -R image_name`

`docker run --name static-site-2 -e AUTHOR="Elhoucine" -d -p 8888:80 seqvence/static-site`

<!-- http://192.168.99.100:5000/ -->

[TUTORIAL](https://github.com/docker/docker-birthday-3/blob/master/tutorial.md#static-site)
