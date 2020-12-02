FROM ubuntu:focal

RUN apt-get update -o Acquire::Retries=30 \ 
&& DEBIAN_FRONTEND=noninteractive apt-get install -o Acquire::Retries=30 -y --no-install-recommends \
clang gcc build-essential wget git python unzip ca-certificates

WORKDIR /home/project

RUN mkdir project && cd project && wget https://github.com/qemu/qemu/archive/stable-4.2.zip && unzip stable-4.2.zip