FROM ubuntu:22.04
SHELL ["/bin/bash", "-c"]
RUN apt update
RUN apt install -y vim
RUN apt install -y net-tools
RUN apt install -y iputils-ping
RUN apt install -y curl
RUN apt install -y wget
RUN apt install -y git
RUN apt install -y build-essential
RUN apt install -y libwebkit2gtk-4.0-dev
RUN apt install -y libssl-dev
RUN apt install -y libgtk-3-dev
RUN apt install -y libayatana-appindicator3-dev
RUN apt install -y librsvg2-dev
RUN curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs >> install_rust.sh && chmod 700 install_rust.sh && ./install_rust.sh -y
ENV PATH="/root/.cargo/bin:${PATH}"
RUN cargo install tauri-cli --version "^1.0.0"
ENTRYPOINT ["/bin/bash"]
