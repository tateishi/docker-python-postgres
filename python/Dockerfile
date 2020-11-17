FROM python:3

RUN apt-get update && apt-get install -y \
        git \
        bash-completion

RUN groupadd -g 1000 ubuntu \
        && useradd -u 1000 -d /home/ubuntu -g ubuntu ubuntu \
        && mkdir -p /home/ubuntu \
        && chown ubuntu:ubuntu /home/ubuntu \
        && chsh -s /bin/bash ubuntu

USER ubuntu
WORKDIR /home/ubuntu
