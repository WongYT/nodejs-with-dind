### introduction
t is combine two docker image those are docker:dind and node:alpine.

### Reference
Reference docker file:
1. docker:dind
https://github.com/docker-library/docker/blob/00de5231b507c989ce900df2ef3f1abf4ce7e19c/17.10/dind/Dockerfile

2. node:alpine
https://github.com/nodejs/docker-node/blob/c75cc560e2642755c6fbb2a53b8716063c0b3806/9/alpine/Dockerfile


### How to use
If you want to run your node code on yueting/nodejs-with-dind, please use multi-service in docker
https://docs.docker.com/engine/admin/multi-service_container/

* 1. start docker service
```
dockerd --host=unix:///var/run/docker.sock --host=tcp://0.0.0.0:2375 --storage-driver=vfs
```

* 2. start nodejs
```
npm start
```
