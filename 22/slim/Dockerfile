FROM erlang:22.3.4.21-slim

RUN apt-get update \
    && apt-get install -y git \
     build-essential

RUN groupadd -g 1000 erlang \
    && useradd -g 1000 -u 1000 -d /home/erlang -s /bin/bash erlang

RUN mkdir -p /home/erlang/app \
    && chown -R erlang:erlang /home/erlang

USER erlang:erlang
VOLUME  /home/erlang
WORKDIR  /home/erlang/app