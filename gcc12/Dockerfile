FROM ubuntu:22.04
SHELL ["/bin/bash", "-c"]
RUN apt update
RUN apt install -y vim
RUN apt install -y net-tools
RUN apt install -y iputils-ping
RUN apt install -y curl
RUN apt install -y git
RUN apt install -y gcc-12
RUN apt install -y g++-12
RUN apt install -y gdb
RUN apt install -y cmake
WORKDIR /root
ENTRYPOINT ["/bin/bash"]