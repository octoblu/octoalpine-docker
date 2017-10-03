FROM octoblu/octoalpine:latest
MAINTAINER Octoblu <docker@octoblu.com>

ENV DOCKER_VERSION 17.09.0-ce
env DOCKER_MACHINE_VERSION 0.12.2

RUN curl -fsSLO "https://github.com/docker/machine/releases/download/v$DOCKER_MACHINE_VERSION/docker-machine-Linux-x86_64" \
  && mv docker-machine-Linux-x86_64 /usr/local/bin/docker-machine \
  && chmod +x /usr/local/bin/docker-machine

RUN curl -fsSLO "https://download.docker.com/linux/static/stable/x86_64/docker-$DOCKER_VERSION.tgz" \
  && tar --strip-components=1 -xvzf "docker-$DOCKER_VERSION.tgz" -C /usr/local/bin \
  && chmod +x /usr/local/bin/docker \
  && rm "docker-$DOCKER_VERSION.tgz"
