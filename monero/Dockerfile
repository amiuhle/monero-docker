FROM ubuntu:16.04

RUN apt-get -y update && apt-get install -y \
  bzip2 \
  curl

RUN curl https://downloads.getmonero.org/cli/monero-linux-x64-v0.10.2.0.tar.bz2 > /tmp/monero.tar.bz2

RUN echo "bf27eb173a775b62716b5fd1d1921f81c8d3b91187b190a22f2a6d82811915fd /tmp/monero.tar.bz2" | sha256sum -c

RUN tar -xf /tmp/monero.tar.bz2 -C /tmp && mv /tmp/monero-v0.10.2/* /usr/local/bin/

