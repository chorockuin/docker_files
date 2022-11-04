FROM ubuntu22.04:1.0.0
SHELL ["/bin/bash", "-c"]
RUN apt install -y build-essential
RUN curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs >> install_rust.sh && chmod 700 install_rust.sh && ./install_rust.sh -y
ENV PATH="/root/.cargo/bin:${PATH}"
RUN cargo install wasm-pack
RUN cargo install trunk
RUN rustup target add wasm32-unknown-unknown
WORKDIR /root
ENTRYPOINT ["/bin/bash"]
