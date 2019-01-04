#Serve static files from docker
#
FROM ubuntu:16.04
MAINTAINER Upma 
USER root
RUN apt-get update
RUN apt-get install -y nginx
RUN rm -v /etc/nginx/nginx.conf
WORKDIR .
ADD nginx.conf /etc/nginx/
ADD index.html /usr/share/nginx/html/
EXPOSE 80
CMD service nginx start

