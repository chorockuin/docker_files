FROM ubuntu:22.04
SHELL ["/bin/bash", "-c"]
RUN apt update
RUN apt install -y vim
RUN apt install -y net-tools
RUN apt install -y iputils-ping
RUN apt install -y curl
RUN apt install -y wget
RUN apt install -y unzip
RUN apt install -y git
RUN apt install -y python3.10
RUN apt install -y pip
WORKDIR /root
RUN wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | apt-key add -
RUN sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list'
RUN apt update
RUN apt install -y google-chrome-stable
RUN wget https://chromedriver.storage.googleapis.com/106.0.5249.61/chromedriver_linux64.zip
RUN unzip chromedriver_linux64.zip
RUN rm chromedriver_linux64.zip
RUN pip install selenium
ENTRYPOINT ["/bin/bash"]
