FROM ubuntu:16.04

RUN apt-get -y update && apt-get install -y \
  curl

RUN curl https://downloads.getmonero.org/monero.linux.x64.v0-10-1-0.tar.bz2 > /tmp/monero.tar.bz2

RUN echo "bf09eea27c957e7e2bdd62dac250888b301d4d25abe18d4a5b930fa7477708c7 /tmp/monero.tar.bz2" | sha256sum -c

RUN tar -xf /tmp/monero.tar.bz2 -C /usr/local/bin/

