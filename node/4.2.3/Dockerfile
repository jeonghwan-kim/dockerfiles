FROM jeonghwan/ubuntu:14.04
MAINTAINER Jeonghwan Kim <ej88ej@gmail.com>

# Install nodejs
RUN curl https://deb.nodesource.com/node_4.x/pool/main/n/nodejs/nodejs_4.2.3-1nodesource1~trusty1_amd64.deb > node.deb \
 && dpkg -i node.deb \
 && rm node.deb

RUN npm install -g pangyp\
 && ln -s $(which pangyp) $(dirname $(which pangyp))/node-gyp\
 && npm cache clear\
 && node-gyp configure || echo ""

RUN apt-get update \
 && apt-get upgrade -y --force-yes \
 && rm -rf /var/lib/apt/lists/*;

# Install forever
RUN npm install forever -g
