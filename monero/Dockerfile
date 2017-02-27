FROM ubuntu:16.04

RUN apt-get -y update && apt-get install -y \
  bzip2 \
  curl

RUN curl https://downloads.getmonero.org/cli/monero-linux-x64-v0.10.2.1.tar.bz2 > /tmp/monero.tar.bz2

RUN echo "9edba6ca91c35c6c2eb6816f9342931c88648de5beb471943ea63d0b16c9a2e4 /tmp/monero.tar.bz2" | sha256sum -c

RUN tar -xf /tmp/monero.tar.bz2 -C /tmp && mv /tmp/monero-v0.10.2.1/* /usr/local/bin/

