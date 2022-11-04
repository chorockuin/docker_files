FROM ubuntu22.04:1.0.0
SHELL ["/bin/bash", "-c"]
RUN wget https://go.dev/dl/go1.19.3.linux-arm64.tar.gz
RUN tar -xvf go1.19.3.linux-arm64.tar.gz
RUN rm go1.19.3.linux-arm64.tar.gz
ENV PATH="/root/go/bin:${PATH}"
WORKDIR /root
ENTRYPOINT ["/bin/bash"]