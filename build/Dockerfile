FROM ubuntu:18.10
WORKDIR /home

ENV LANG C.UTF-8
ENV LC_ALL C.UTF-8

ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update
RUN apt-get -y install \
    build-essential \
    automake \
    golang
    
RUN rm -rf /var/lib/apt/lists/*