FROM ubuntu

RUN apt-get update && apt-get -y upgrade && apt-get install -y git build-essential gcc bc cmake libssl-dev mc nano unzip

RUN mkdir /opt/pol

RUN git clone https://github.com/polserver/polserver.git /root/polserver

WORKDIR /root/polserver/lib

RUN tar xjf boost_1_55_0.tar.bz2

WORKDIR /root/polserver/pol-core/bin-build

RUN ./build_linux.sh

WORKDIR /opt/pol

VOLUME /opt/pol

EXPOSE 2593 5000
