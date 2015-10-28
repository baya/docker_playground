# docker build -t baya/redis .
# docker run -d -p 6379 --name redis baya/redis
# redis-cli -h 192.168.99.100 -p 32775
# docker inspect -f '{{.NetworkSettings.IPAddress}}' redis
FROM ubuntu
MAINTAINER Kayak Jiang kayak.jiang@gmail.com
ENV REFRESHED_AT 2015-10-21
RUN apt-get update
RUN apt-get -y install redis-server redis-tools
EXPOSE 6379
ENTRYPOINT ["/usr/bin/redis-server"]
CMD []