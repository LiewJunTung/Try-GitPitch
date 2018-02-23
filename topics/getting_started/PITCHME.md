## Getting Started

Step 1: Install Docker
+++

Step 2: Pull images

```bash
$ docker pull nginx
```
+++
Step 3: Run

```bash
$ docker run --name nginx-server -d -p 8080:80 nginx
```
+++
Step 4: Run

```bash
$ docker run --name light-nginx-server -d -p 8089:80 nginx:alpine
```
+++
To break it down

```bash
$ docker run \
--name light-nginx-server \
-d \
-p 8089:80 \
nginx:alpine
```
@[1](using the Docker's __run___ command)
@[2](give the container a unique name to run it later)
@[3](-d means detach mode, so that we can use the terminal after running this command)
@[4](-p maps the port from the port to the container. HOST_PORT:CONTAINER_PORT)
@[5](name of the image)
+++
To see the current process

```bash
$ docker ps
```