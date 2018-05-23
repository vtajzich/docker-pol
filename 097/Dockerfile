FROM ubuntu

RUN apt-get update && apt-get -y upgrade && apt-get install -y mc nano unzip

ADD pol.zip /opt/
RUN unzip /opt/pol.zip -d /opt/ && rm /opt/pol.zip

WORKDIR /opt/pol

#VOLUME /opt/pol

EXPOSE 2593 5000
