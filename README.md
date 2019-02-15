My fork of nimmis's Alpine microcontainer with Python. Don't use this in production

based on Alpine 3.8 and Python 2/3
PIP is also installed.

### Examples

This images are build on robotfactory/alpine-micro which are a modified version of Alpine with a working 
init process, and a working cron, logrotate  and syslog. Services are started with
runit daemon.

#### starting the container as a daemon

	docker run -d --name python robotfactory/alpine-python

This will start the container with nginx process runnung, access the container with

	docker exec -ti python /bin/sh

### TAGs

This image contains version 2.x and 3.x, the versions are robotfactory/alpine-python:<tag> where tag is

| Tag    | Python Version | Container size |
| ------ | ---------- | -------------- |
| latest | latest (atm 3.x) |
| 2    | 2.7.11 |
| 3  | 3.5.1 |
