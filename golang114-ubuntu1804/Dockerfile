FROM ubuntu:18.04

MAINTAINER Masataka Hisasue

RUN apt update -y && apt upgrade -y && apt install -y software-properties-common && \
    add-apt-repository -y ppa:longsleep/golang-backports && \
    apt update -y && apt install -y golang-1.14 && \
    echo "export PATH=/usr/lib/go-1.14/bin:$PATH" > $HOME/.bashrc && \
    mkdir /root/go

WORKDIR /root

CMD ["/bin/bash"]
