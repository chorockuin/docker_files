FROM ubuntu:22.04
SHELL ["/bin/bash", "-c"]
RUN apt update
RUN apt install -y vim
RUN apt install -y net-tools
RUN apt install -y iputils-ping
RUN apt install -y curl
RUN apt install -y git
RUN apt install -y wget
RUN apt install -y unzip
RUN mkdir /root/volume
WORKDIR /root
ENTRYPOINT ["/bin/bash"]
