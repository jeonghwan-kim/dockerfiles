FROM jeonghwan/ubuntu:14.04
MAINTAINER Jeonghwan Kim <ej88ej@gmail.com>

# Install mysql-server-5.6
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update \
  && apt-get install -y mysql-server-5.6 \
  && service mysql start
EXPOSE 3306
