# docker build -t baya/sinatra .
# docker run -d -p 4567 --name webapp -v $PWD/webapp:/opt/webapp baya/sinatra
# docker logs -f webapp
# docker top webapp
FROM ubuntu
MAINTAINER Kayak Jiang kayak.jiang@gmail.com
ENV REFRSHED_AT 2015-10-21

RUN apt-get update
RUN apt-get -y install ruby ruby-dev build-essential redis-tools
RUN gem install --no-rdoc --no-ri sinatra json redis

RUN mkdir -p /opt/webapp

EXPOSE 4567

CMD ["/opt/webapp/bin/webapp"]