 Alpine microcontainer with Python

This is a micro docker container [![](https://badge.imagelayers.io/nimmis/alpine-python:latest.svg)](https://imagelayers.io/?images=nimmis/alpine-python:latest) based on Alpine 3.3 and Python 2/3
PIP is also installed.

### Examples

This images are build on nimmis/alpine-micro which are a modified version of Alpine with a working 
init process, and a working cron, logrotate  and syslog. Services are started with
runit daemon, for more information about that see [nimmis/alpine-mico](https://registry.hub.docker.com/u/nimmis/alpine-micro/)

#### starting the container as a daemon

	docker run -d --name python nimmis/alpine-python

This will start the container with nginx process runnung, access the container with

	docker exec -ti python /bin/sh

### TAGs

This image contains version 2.x and 3.x, the versions are nimmis/alpine-python:<tag> where tag is

| Tag    | Python Version | Container size |
| ------ | ---------- | -------------- |
| latest | latest (atm 1.6) | [![](https://badge.imagelayers.io/nimmis/alpine-python:latest.svg)](https://imagelayers.io/?images=nimmis/alpine-python:latest) |
| 2    | 2.7.11 | [![](https://badge.imagelayers.io/nimmis/alpine-python:2.svg)](https://imagelayers.io/?images=nimmis/alpine-python:2) |
| 3  | 3.5.1 | [![](https://badge.imagelayers.io/nimmis/alpine-python:3.svg)](https://imagelayers.io/?images=nimmis/alpine-python:3) |
