FROM ubuntu:18.04

RUN apt-get update && apt-get install -y curl build-essential git -y

RUN useradd -ms /bin/bash balena

RUN usermod -aG sudo balena

RUN apt-get install docker.io -y

RUN usermod -aG docker balena

RUN curl -L https://github.com/docker/compose/releases/download/1.23.0-rc3/docker-compose-Linux-x86_64 -o /usr/local/bin/docker-compose && chmod +x /usr/local/bin/docker-compose

RUN apt-get install libssl-dev -y

RUN apt-get install nodejs -y

RUN apt-get install npm -y

RUN git clone https://github.com/balena-io/open-balena.git ~/open-balena
