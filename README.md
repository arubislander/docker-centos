# docker-centos
Dockerfile for CentOS container for development purposes

[Build Status]

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
