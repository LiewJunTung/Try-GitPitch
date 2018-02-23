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
@[1]
@[2]
@[3]
@[4]
@[5]
+++
To see the current process

```bash
$ docker ps
```