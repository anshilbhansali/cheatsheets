## Docker cheatsheet

```sh
$ docker image ls
$ docker container ls
$ docker ps -a
$ docker run -it <imageID> bash - Start a container from an image
$ docker exec -it <containerID> bash - Enter a running container
$ docker logs <containerID> - see logs of container
$ docker container kill $(docker ps -q) - kill all running containers
$ sudo docker kill $(sudo docker container ls -q --filter name=<query>) - kill all containers with name having query
$ sudo docker exec -it $(sudo docker container ls -q --filter name=<query>) bash
```

## Virtual Env cheatsheet
Create virtual environment
List envs
Activate/Enter venv
```sh
$ python3 -m venv ./<venv-name>
$ ls
$ source ./<venv-name>/bin/activate
$ deactivate
```
