dockerfiles-centos-basic
==========================

CentOS 7 dockerfile for infrastructure services

To build:

Copy the sources down -

```
# docker build -rm -t uriahfeng/docker-basic-image:latest .
```

To run:

```
# docker run -it -d --privileged --volume=/sys/fs/cgroup:/sys/fs/cgroup:ro uriahfeng/docker-basic-image:latest
```

Check the that the image launched successfully

```
# docker ps
CONTAINER ID        IMAGE                                 COMMAND             CREATED             STATUS              PORTS                    NAMES
b1296df1a4e8        uriahfeng/docker-basic-image:latest  /usr/sbin/init       3 seconds ago       Up 1 seconds                                 basic_system         
```
