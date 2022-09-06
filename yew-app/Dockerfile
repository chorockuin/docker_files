FROM yew:0.1.0
RUN cd /root && git clone https://github.com/chorockuin/yew-app.git
ENTRYPOINT ["trunk", "serve"]
CMD ["/root/yew-app/index.html", "--release", "--address", "0.0.0.0"]