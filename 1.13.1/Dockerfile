FROM octoblu/octoalpine:latest
MAINTAINER Octoblu <docker@octoblu.com>

RUN curl -fsSLO https://github.com/docker/machine/releases/download/v0.9.0/docker-machine-Linux-x86_64
RUN mv docker-machine-Linux-x86_64 /usr/local/bin/docker-machine
RUN chmod +x /usr/local/bin/docker-machine

RUN curl -fsSLO https://get.docker.com/builds/Linux/x86_64/docker-1.13.1.tgz
RUN tar --strip-components=1 -xvzf docker-1.13.1.tgz -C /usr/local/bin
RUN chmod +x /usr/local/bin/docker
