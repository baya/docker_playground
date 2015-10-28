# jekyll dockerfile
# docker build -t baya/jekyll .
FROM ubuntu
MAINTAINER Kayak Jiang <kayak.jiang@gmail.com>
ENV REFRSHED_AT 2015-10-28


RUN apt-get -yqq update
RUN apt-get -yqq install curl
RUN curl --silent --location https://deb.nodesource.com/setup_4.x | sudo bash -
RUN apt-get -yqq install ruby ruby-dev make nodejs
RUN gem install --no-rdoc --no-ri jekyll

VOLUME /data
VOLUME /var/www/html
WORKDIR /data

ENTRYPOINT ["jekyll", "build", "--destination=/var/www/html"]



