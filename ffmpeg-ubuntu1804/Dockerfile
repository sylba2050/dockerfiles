FROM ubuntu:18.04

MAINTAINER Masataka Hisasue

RUN apt -y update && apt -y upgrade && apt install -y software-properties-common && \
    add-apt-repository -y ppa:jonathonf/ffmpeg-4 && \
    apt -y update && \
    apt install -y ffmpeg=7:4.3-2~18.04.york0

CMD ["/bin/bash"]
