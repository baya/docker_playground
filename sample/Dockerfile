# wget https://raw.githubusercontent.com/jamtur01/dockerbook-code/master/code/5/sample/nginx/global.conf
# wget https://raw.githubusercontent.com/jamtur01/dockerbook-code/master/code/5/sample/nginx/nginx.conf
# docker build -t baya/nginx ./
FROM ubuntu
MAINTAINER Kayak Jiang "kayak.jiang@gmail.com"
ENV REFESHED_AT 2015-10-20
RUN apt-get update
RUN apt-get -y -q install nginx
RUN mkdir -p /var/www/html
ADD nginx/global.conf /etc/nginx/conf.d/
ADD nginx/nginx.conf /etc/nginx/nginx.conf
EXPOSE 80