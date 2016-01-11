# docker-centos

[![Docker Stars](https://img.shields.io/docker/stars/arubislander/centos.svg)](https://hub.docker.com/r/arubislander/centos/)
[![Docker Pulls](https://img.shields.io/docker/pulls/arubislander/centos.svg)](https://hub.docker.com/r/arubislander/centos/)
[![ImageLayers Size](https://img.shields.io/imagelayers/image-size/arubislander/centos.svg)](https://hub.docker.com/r/arubislander/centos/)
[![ImageLayers Layers](https://img.shields.io/imagelayers/layers/arubislander/centos.svg)](https://hub.docker.com/r/arubislander/centos/)

Dockerfile for CentOS container for development purposes

This image comes with the following packages preinstalled:
`automake
gcc
gcc-c++
glibc-devel.i686
libgcc.i686
libstdc++.i686
make
nano`

This makes it possible to use this image to build containers that can compile 64 bit and 32 bit ELF files that will run on CentOS and RHEL

Example:
`docker run -it -h docker-centos --name=docker-centos -v `\``pwd`\``/centos:/home/docker -w /home/docker arubislander/centos:6 /bin/bash`
