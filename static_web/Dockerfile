# Version 0.0.1
FROM ubuntu
MAINTAINER Kayak Jiang "kayak.jiang@gmail.com"
RUN apt-get update
RUN apt-get install -y nginx
RUN apt-get install -y curl
RUN echo 'Hi, I am in your container' > /usr/share/nginx/html/index.html
ENTRYPOINT ["/usr/sbin/nginx"]
CMD ["-h"]
EXPOSE 80


