FROM jeonghwan/ubuntu:14.04
MAINTAINER Jeonghwan Kim <ej88ej@gmail.com>

# Install mongodb 3.2
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv EA312927 \
  && echo "deb http://repo.mongodb.org/apt/ubuntu trusty/mongodb-org/3.2 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.2.list \
  && apt-get update \
  && apt-get install -y mongodb \
  && service mongodb start
EXPOSE 27017