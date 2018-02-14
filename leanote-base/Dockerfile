FROM mongo:latest

RUN apt-get update
RUN apt-get install -y curl && \
    curl -L http://sourceforge.net/projects/leanote-bin/files/2.6/leanote-linux-amd64-v2.6.bin.tar.gz/download >> \
    /usr/local/leanote-linux-amd64.bin.tar.gz

RUN tar -xzvf /usr/local/leanote-linux-amd64.bin.tar.gz -C /usr/local
