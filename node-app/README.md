# Basic Node App using docker

## How to Build this image
```bash
docker build . -t actionanand/node-app:Version
```

## How to Pull this image from docker hub
```shell
docker pull actionanand/node-app
```
or
```bash
docker pull actionanand/node-app:Version
```

## How to run this image

```shell
docker run -d -p 3000:80 --rm --name node-app actionanand/node-app:Version
```

## Other useful commands

* `docker ps`: **List** all **running** containers
  * `-a` : **List** all **containers** - including **stopped** ones
* `docker images` : **List** all **locally stored images**
* `docker stop my_container` : Stops the running container with the name 'my_container' or ID
* `docker rm CONTAINER` : **Remove** a container with name `CONTAINER` (you can also use the
`container id`). You can use multiple container name or ID followed by white space. SO `docker rm CONTAINER_1 CONTAINER_2 CONTAINER_3`
* `docker rmi IMAGE` : **Remove** an image by name / id. You can use multiple image name or ID followed by white space.
* `docker container prune` : **Remove** all **stopped** containers
* `docker image prune` : **Remove** all **dangling** images (untagged images)
  * `-a` : **Remove** all **locally stored** images
* `docker attach container_name`: Will attach the container again
* `docker logs container_name`: Will print logs by the container
  * `-f` : follow tag will attach it again to print the future logs in terminal

[GitHub - Docker_Playground](https://github.com/actionanand/docker_playground)